<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

!!! note

    The following text is an attempt to explain why we use a review process before creating new ICAO aircraft type codes

We target to have all **official ICAO codes** from [www.icao.int](http://www.icao.int/publications/DOC8643/Pages/Search.aspx) in our database.
The ICAO database is one of our main references.

* sometimes it is hard to understand why or why not ICAO created a new entry for a certain aircraft type
* some entries of the ICAO database are duplicates of other entries.
  This seems to have technical reasons and we will try to eliminate those duplicates (if they are reported)
  * general rule: **All entries** of [www.icao.int](http://www.icao.int/publications/DOC8643/Pages/Search.aspx) **minus duplicates** are supposed to be in the *swift* Datastore
  * **IATA codes**: There are cases where IATA distinguishes two aircraft types, while ICAO does not.
  This means IATA uses are more detailed scheme and we (normally) create those extra entries.

## Code descriptions

* we have 3 description fields which can be used to describe the aircraft.
  As those fields are searchable such descriptions will help to find the most appropriate entry
* normally we will use those fields to provide the company aircraft types
* in cases where there are more detailed company codes (more detailed than the ICAO and IATA entries) we need to decide case by case if it makes sense to create multiple entries, or rather use one of the existing entries.
  This decision depends on many factors:
  * is there a visual difference among those company types?
  * is the aircraft frequently used in flight simulation?
  * are many distributions supporting this aircraft?

Remark: As it is easier to later merge entries (than to split them), sometimes it makes sense to create a new entry if not 100% sure.
