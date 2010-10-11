ec2-delete-registered-snapshot
==============================

This is a simple timesaver script for deleting registered snapshots by
first unregistering the ami and then deleting the snapshot.
I use it for the EBS based backups that I create by another script.

Usage:
------
ec2-delete-registered-snapshot snap-12345678


The ec2-descripe-snapshots output expected from this script is as follows:
SNAPSHOT  snap-12345678   vol-90abcdef    completed   2010-07-27T21:52:51+0000    100%    266627911898    15  Created by CreateImage(i-87654321) for ami-abcdefab from vol-90abcdef

