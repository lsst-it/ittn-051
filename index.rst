..
  Technote content.

  See https://developer.lsst.io/restructuredtext/style.html
  for a guide to reStructuredText writing.

  Do not put the title, authors or other metadata in this document;
  those are automatically added.

  Use the following syntax for sections:

  Sections
  ========

  and

  Subsections
  -----------

  and

  Subsubsections
  ^^^^^^^^^^^^^^

  To add images, add the image file (png, svg or jpeg preferred) to the
  _static/ directory. The reST syntax for adding the image is

  .. figure:: /_static/filename.ext
     :name: fig-label

     Caption text.

   Run: ``make html`` and ``open _build/html/index.html`` to preview your work.
   See the README at https://github.com/lsst-sqre/lsst-technote-bootstrap or
   this repo's README for more info.

   Feel free to delete this instructional comment.

:tocdepth: 1

.. Please do not modify tocdepth; will be fixed when a new Sphinx theme is shipped.

.. sectnum::

.. TODO: Delete the note below before merging new content to the master branch.

.. note::

   **This technote is not yet published.**

   To Move Jira Projects from Tucson On-Premise to Atlassian Jira Cloud

.. Add content here.
.. Do not include the document title (it's automatically added from metadata.yaml).

An Evaluation of Projects
=========================
- Will it Move to Cloud or Retired/Deleted
- Is it only for Construction
- Will it move to Operations
- Plan to transition to NOIRLab Jira

Information Topics
==============
Are No Longer Valid: https://jira.lsstcorp.org/browse/RFC-751 & https://ittn-035.lsst.io

Do we need an RFC?

Cloud and Migration Information 
-------------------------------
- https://www.atlassian.com/cloud/myths/overview
- https://www.atlassian.com/cloud/guide
- Data Application footprint <get details but no more than ~200G>

Cloud Security
--------------
- https://support.atlassian.com/security-and-access-policies/docs/how-to-keep-my-organization-secure/
- https://support.atlassian.com/security-and-access-policies/docs/understand-atlassian-access/
- https://blog.isostech.com/atlassian-access/crowd-what-you-need-to-know

Our Jira Cloud Instance
========================
RubinObs has a Cloud Instance is Jira Software: http://rubinobs.atlassian.net/
- List of Site Administrators to manage the cloud instance and all projects within

General Topics
============
- Outage of General Services
- Outage Isolating the Base-Summit from Jira Cloud
- Migrating to another Jira-Like Service
- Backups of our Data in case of lock outs
- Security and User Groups

What Directory Service(s) are we to use?
=======================================
Examples Existing AD-Tucson, Atlasian, AD-NOIRLab, Github, Google, combinations of these or others

Considerations
---------------
- Existing Users are mostly Crowd-AD
- No Crowd Users
- Some local Jira Users (same with Confluence)
- Not all users of Jira have Github or G-Suite profiles/accounts
- Not all users are within the AURA/RubinObs Ecosystem
- Plan on transfer to NOIRLab Jira

Investigate
-----------
- Continue with AD-Tucson in cloud?
- Requires isolated RODC in DMZ (safe enough?)
- Can group membership support contain users from various Directory Services (been a problem with Crowd)
- How will the Project structure groups to improve the method used today?
- Use 2FA for site changes or sensitive projects?

Move all Projects “At Once” or “One-At-Time”
=========================================
- Evaluate the different methods

URL Redirect 
==================
- Will Issue links from On-Premise Map Well to Cloud Instance
- Is simple CNAME Record sufficient or Map-Rules required

Backup and Recovery
========================
- Any concerns about billing and account lock out?
- Ransomware affects Cloud
- Extended Outage when Summit/Base/Operations is in maintenance or operation mode

Tasks
==============
- Define List of Stakeholder Groups and Rep(s)/Liaison(s) 
  DM-SQRE Frossie E
  SE Austin R
  Camera ?
  PMO Budget and Schedule ?
  Pre-Operations Bob B
  NOIRLab Chris M
  General Users ?
  Consumer agents, bots, or services?
  Others ?
  

Prepare Test Migrations
-----------------------
- Owner of Site should prepare a document of actions/tests for IT to perform as first check
- Owner of Site should have Acceptance Requirements
- Owner of Site should prepare the project for migration
    - Project may fail pre-flight and action will be required
    - Purge non-essential data

Configure Infrastructure for Directory Service(s)
-------------------------------------------------
- This may be required before testing or only to prepare for migration
- Test the various login methods
- Test various access and group membership of those logins
- What sort of “sync” between the Directory Service Account and Jira Account Profile
	- If I login as iaingoodenow to the account using AD igoodenow in Jira project X
- Get a list of Local Users of Jira (and Confluence)
- What about DB Logins like JiraRO used by GC (not sure who now)?

First-Attempt Migrations
------------------------
- Basic Import Process and Tests
- Acceptance Tests to Perform
- Develop FAQ
- Need a list of which Add-ons / project?

Prepare and Execute All or Iterate the Actual Migration
---------------------------------------------------
- Formal Testing
  - Stakeholders/Owners need to exercise the work flow and overall functionality
- Need to Know New Link Locations - How to Handle Communication from IT and Owners to Stakeholders

Close out old system
--------------------
- No project should exist
- Assumed data will be purged and guest deleted    


.. .. rubric:: References

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa
