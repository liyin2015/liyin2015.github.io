---
published: true
title: Mac link gcc
layout: post
---
After installed gcc with brew, do the following steps to link it till gcc --version can find the information.

At first, go to /usr/local/Cellar/gcc/5.3.0/bin to check, we can see two files with name gcc-5 and g++-5

$>cd /usr/local/Cellar/gcc/5.3.0/bin
$>ln -s gcc-5 gcc
$>ln -x g++-5 g++
$> cd ~
$>brew link gcc

If you already linked gcc before, do brew unlink gcc, and use brew link gcc to link again.

