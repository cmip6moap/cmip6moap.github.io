---
title: Creating an account on JASMIN
date: 2021-05-06
authors:
 - "[James Thomas](https://github.com/jatonline/) ([Jean Golding Institute](https://www.bristol.ac.uk/golding/))"
layout: resource
---

<div class="lead" markdown="1">
# A guide to creating an account on JASMIN for our hackathon

You can take part in the hackathon **whether or not** you have your own JASMIN
account.

* If you **have an account already**, then please ensure you have access to the
  services below, before the start of the hackathon
* If you **do not have an account**, then you will be allocated a temporary
  account (called a *training account*) to be used for the duration of the
  hackathon and you do not need to follow this guide

If you are a project lead, or intend to work on the hackathon outputs after the
event has finished, then we do ask that you create your own JASMIN account.
</div>

## Overview
{:.no_toc}

In this guide we'll cover:

* Table of contents
{:toc}

The JASMIN team have also created an excellent [workshop and associated training content](https://github.com/cedadev/jasmin-workshop)
that give an excellent overview of JASMIN.

These materials include:

* [How to set up SSH on your machine](https://github.com/cedadev/jasmin-workshop/tree/master/exercises/ex00)
* [How to connect to JASMIN](https://github.com/cedadev/jasmin-workshop/tree/master/exercises/ex01)
* [How to execute code on a scientific analysis server](https://github.com/cedadev/jasmin-workshop/tree/master/exercises/ex02)

There are also support videos and cheat sheets available through these guides.

If you are not familiar with JASMIN we suggest you will also find these very
helpful. We did!

## Applying for a user account

The JASMIN website has [instructions on applying for an account](https://www.jasmin.ac.uk/users/access/),
including the eligibility criteria.

In summary:

* [Use the JASMIN Accounts Portal](https://accounts.jasmin.ac.uk/application/new/)
  to apply for a new account

## Getting access to the right services

Once activated, you can use your JASMIN account to access numerous different
services.

The accounts portal will show you [which services you have been granted access to](https://accounts.jasmin.ac.uk/services/my_services/).

Please ensure you have been granted user-level access to:

* [`jasmin-login`](https://accounts.jasmin.ac.uk/services/login_services/jasmin-login/)
  – the ability to login via SSH, access scientific analysis servers, transfer
    servers and the LOTUS job scheduling system
* [`jupyter-notebooks`](https://accounts.jasmin.ac.uk/services/additional_services/jupyter-notebooks/)
  – the ability to use the Jupyter Notebooks service that we will be using
    throughout the hackathon
* [`xfer-sp`](https://accounts.jasmin.ac.uk/services/additional_services/xfer-sp/)
  – the ability to transfer data in and out of JASMIN if your institution does
    not provide a VPN for access to JASMIN
* [`cop26_hackathon_bristol`](https://accounts.jasmin.ac.uk/services/group_workspaces/cop26_hackathon_bristol)
  – the ability to access and write data within a shared storage area for the
    duration of the hackathon

## Ensuring you have SSH access

You can access the Jupyter Notebooks service through a web browser just using
your JASMIN password, however to be able to login via SSH you will need to set
up an SSH public/private key pair.

If you're not sure how to do this, consult the [JASMIN documentation on SSH key pairs](https://help.jasmin.ac.uk/article/185-generate-ssh-key-pair).

Once you have an SSH key pair, you need to:

* [Enter your SSH *public* key](https://accounts.jasmin.ac.uk/account/profile/update_ssh_key/)
  into the JASMIN Accounts Portal
* [Check that you can login](https://help.jasmin.ac.uk/article/187-login) to one
  of the scientific analysis servers using *SSH agent-forwarding*

  > Note: in order to SSH to most of the JASMIN login servers, you will normally
  > need to be located **within a UK academic network**, or be logged on to an
  > **academic VPN** that will forward connections to JASMIN via the academic
  > network. The [University of Bristol F5 VPN](https://uob.sharepoint.com/sites/itservices/SitePages/vpn-connect.aspx),
  > for instance, should meet this criteria.
  >
  > If this is not the case, you should still be able to access JASMIN as long
  > as you login via `login2.jasmin.ac.uk`.

  From your personal computer, you will run a set of commands similar to the
  following:
  <pre>
  eval $(ssh-agent)
  ssh-add <abbr title="The path to your SSH private key">~/.ssh/id_rsa_jasmin</abbr>
  ssh -A <abbr title="Your JASMIN username">USERNAME</abbr>@<abbr title="The address of the login server you are using">login2.jasmin.ac.uk</abbr>
  </pre>

  Then from the JASMIN login server that you have just logged in to:
  <pre>
  ssh sci1
  </pre>

  If the above command was successful, you are now inside on of the scientific
  analysis servers.

## Ensuring you have Jupyter Notebook access

Check that you can login to the [JASMIN Notebook Service](https://notebooks.jasmin.ac.uk),
create a new notebook and execute some Python code.

There will be a two-step verification process using your institution email
address.

## Ensuring you have access to the hackathon Group Workspace

Check that you can access the directory `/gws/pw/j05/cop26_hackathons/bristol`,
either using the Notebook Service or a Scientific analysis server.

For example, in a Jupyter Notebook you could execute a cell containing:
<pre>
!ls -al /gws/pw/j05/cop26_hackathons/bristol
</pre>

Or if connecting via SSH, you could type the following at the command line:
<pre>
cd /gws/pw/j05/cop26_hackathons/bristol
ls -al
</pre>

Note that you will not be able to access the upper level `cop26_hackathons`
directory, only the `bristol` directory beneath this.
