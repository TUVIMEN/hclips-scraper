# hclips-scraper

A bash script for archiving hclips videos and users metadata in json.

## Requirements

 - [reliq](https://github.com/TUVIMEN/reliq)
 - [jq](https://github.com/stedolan/jq)

## Installation

    install -m 755 hclips-scraper /usr/bin

## Json format

Here's example of a [videos](videos-example.json) and [users](users-example.json).

## Usage

Results will be saved in files named by their sha256 hash of urls and placed in DIR, files contain multiple results.

Download metadata of videos in DIR using 8 threads

    hclips-scraper -t 8 -v DIR

Download metadata of users in DIR

    hclips-scraper -u DIR
