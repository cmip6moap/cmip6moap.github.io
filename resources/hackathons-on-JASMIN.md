---
title: Running a Hackathon on JASMIN
date: 2021-03-04
permalink: /resources/hackathons-on-jasmin/
layout: post
---

<div class="lead" markdown="1">
# A guide to running an event on the JASMIN data analysis facility

This guide is based on the experiences of the University of Bristol in
organising a CMIP6 Hackathon in association with the Met Office Academic
Partners. It describes how we used the JASMIN platform, the decisions we took
and why, and advice for others running similar events.
</div>

## User accounts

As a service providing support to NERC and the environmental science community,
including access to the CEDA archive, JASMIN is typically used in one of two
ways:

1. Interactive compute e.g. running scripts from command line using the
   scientific analysis servers – they come with a lot of software and packages
   pre-installed, have read access to the CEDA archive and read/write to group
   workspaces and personal home directories
2. Batch compute using the LOTUS job system – there are both CPU and GPU nodes
   available and are best suited to group workspaces where processing of 100s of
   TBs of data is required Getting access to JASMIN if you are not an existing
   account holder is traditionally a process that takes some time, involving
   getting approval for your account, setting up two-factor authentication, SSH
   public key authentication etc. These can be a barrier to some users,
   especially with a short timescale.

### Accelerating access for event users

We decided to use [JASMIN Notebook Service](https://notebooks.jasmin.ac.uk/), a
relatively new service called which allows Python 3 to be run through the
browser. This is a modified JupyterLab with e.g. terminal access removed.
Different packages can be installed using conda.

We also opted to offer every participant a “training account” on JASMIN,
although those with existing accounts can use them instead.

This is a simpler and faster way for new users to get onto JASMIN for the event,
because:

* Training accounts are assigned to a user for the length of the hackathon and
  then switched off afterwards, or if users have JASMIN accounts then they can
  apply to have the Notebook Service added to their account
* Users are sent credentials via email for the Notebook Service and (optionally)
  can download an SSH key pair if they want to have SSH access
* Each user gets read access to the public parts of the CEDA archive (inc.
  CMIP6) and read/write to 100GB of home directory

However, there are some drawbacks:

* Only Python 3 can be used, and not other languages such as R
* Read access to group workspaces has to arranged by prior permission of the
  group owners, and write access is not possible
* At the end of the hackathon, users will need to have copied the code that they
  need off the training account, or committed it to Git (preferred), because it
  will later be removed[^1]

For promising projects, users could be issued with proper JASMIN accounts
created at the end of the hackathon, to allow them to continue working.

## Available resources

At time of writing, the JASMIN Notebook Service runs on a Kubernetes cluster
with three nodes, with up to 72 CPUs and 1.1TiB RAM available. When a user logs
into the JASMIN Notebook Service, a new notebook server is started specifically
for them. This notebook server is guaranteed 1 CPU and 4GB RAM, although can use
up to 4 CPUs and 16GB RAM if the resources are available in the cluster. There
are no specific limits on the number of concurrent users, however if there are
no resources available in the cluster then the user’s notebook server will fail
to start.

Note that the following are **not** currently available:

* JupyterLab plugins (e.g. Git)
* JupyterLab terminal access (commands can be run via a notebook magic, but will
  not be able to interact with programs – full terminal access requires the use
  of SSH)
* A Dask back-end for parallel tasks within the Notebook Service

## Timescale considerations

Date              | Actions
----              | -------
4 months before   | Engage with JASMIN, check dates do not clash with other events<br> Request research topic idea from researchers
3 months before   | Finalise proposed research topics<br> Participant applications open
2 months before	  | Deadline for participant applications
1.5 months before | Finalise participants<br> Provide list of participants to JASMIN
1 month before    | Provide welcome packs to participants<br> Finalise example notebooks / repositories
1 week before     | Training accounts will be set-up by JASMIN<br> Provide drop-in sessions with participants, ensure they can connect
Hackathon date    | 
1 week after      | Remind participants to move data off system

#### Notes

[^1]: It is anticipated the code will be the most important thing, as the data
      can be regenerated. There is also the option of making all the code and
      data public for a period of time (e.g. a month) in case users need longer
      to download their code/data.
