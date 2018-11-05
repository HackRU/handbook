# Sponsor Platform

**This is a proposal and may never exist as a standalone project, but as a set of features.**

PLease comment on it. This file will disappear into TO-DOs on the following projects if the RFC
is approved:
 - a standalone project.

We expect this for Spring 2019.

## Description
*What is the purpose of this project?*

This project aims to let sponsors interact with hackers more easily on the day of.
The basic idea is to let sponsors scan QR codes of hackers to allow them access to resumes.
The scanner is allowed only for sponsors of a particular tier.

We hope to include a few more features:
 - A feature to star emails scanned for sponsors to remember. We may also allow them to add notes
   if not custom labels.
 - A map detailing the table location and the finance welcome pack in the app.
 - A listing of hacks that applied for the sponsors prizes.

## Inspiration
*How did this project come to be?*

HackGT.

## Installation Guide
*How do the users get this up and running?*

**This is a proposal.**

Here are a few tentative steps to get this to work:
1. Add sponsors to LCS. We'll have to use magic links to set them as sponsors and
   track their sponsorship level.
1. Based on the sponsor level, the apps will have to allow the sponsors to scan QR codes
   to receive resumes. This also means that the apps will have to access the S3 bucket for resumes.
1. Add sponsors to the day-of map (as a convenience)
1. There may have to be a "card" on the frontend for sponsor users to see their tier and status.

## Example Uses

Smoother contact sharing on the day of: a hacker will just have to have their QR scanned to share their resume and contact information with the sponsors.
Sponsors may also use this to track day-of information including their table location (as a part of the map on the app).

## Style Guide

N/A

## TO-DO List

Get the RFc approved by finance.

## Links to Further docs

N/A for now.

## Other crazy extensions

These are just ideas. Based on past conversations with finance or experience, they are unlikely to be
useful or worth the effort.

 - Allow sponsors to upload contracts through the website.
 - A way for sponsors to add web-hooks LCS can call on QR scans.
 - clara@mlh.io, but for HackRU.
