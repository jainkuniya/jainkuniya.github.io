---
published: false
title: "Hands on with Postgresql vacuum"
layout: post
date: 2020-02-02 02:04
image: /assets/mount-batur/mount-batur-top.jpg
headerImage: true
tag:
  - mount-batur
  - nature
  - clouds
  - hills
  - mountains
  - volcano
category: blog
star: true
author: vishwesh
description: Looking for a trek in Bali? Here is all the information you need to know before you start.
---

- **VACUUM**: 
    - Removes dead row versions in tables and indexes and marks the space available for future reuse.
    - Run in parallel to `SELECT, INSERT, UPDATE, and DELETE`
    - But won't be able to `ALTER TABLE`
- **VACUUM FULL**:
    - Requires exclusive lock on table.
    - Actively compacts tables by writing a complete new version of the table file with no dead space.
    - Also requires more disk space, as new copy is created.
- **TRUNCATE**: 
    - Removes entire content immediately, prefered over `DELETE` followed by `VACUUM`
- **MULTIVERSION CONCURRENCY CONTROL**:
    - to provide concurrent access to the database and in programming languages to implement transactional memory
    
    