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
Note  - Are No Longer Valid
https://jira.lsstcorp.org/browse/RFC-751
https://ittn-035.lsst.io/
Do we need an RFC?

Cloud and Migration Information 
—————————————————————
- https://www.atlassian.com/cloud/myths/overview
- https://www.atlassian.com/cloud/guide
- Data Application footprint <get details but no more than ~200G>

Cloud Security
———————————
- https://support.atlassian.com/security-and-access-policies/docs/how-to-keep-my-organization-secure/
- https://support.atlassian.com/security-and-access-policies/docs/understand-atlassian-access/
- https://blog.isostech.com/atlassian-access/crowd-what-you-need-to-know

.. .. rubric:: References

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa
