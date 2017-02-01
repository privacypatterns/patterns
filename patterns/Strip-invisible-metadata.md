    {%hyde

    title: "Strip Invisible Metadata"
    excerpt: "Strip potentially sensitive metadata that isn't directly visible to the end user."
    status: draft
    display_in_list: True
    type: pattern
    categories:
        - metadata
        - minimization
        - exif
        - location
        - media

    %}

[TOC]

## Intent

## Context

When a service requires a user to import data from external sources (eg.
pictures, tweets, documents) different types of metadata may be 
transmitted. Users may not be aware of the metadata as it can be
automatically generated or not directly visible. Services might be
inadvertently responsible for exposing private metadata, or going
against users' expectations.

## Problem

Users are not always fully aware of the various kinds of metadata
attached to files and web resources they share with online services.
Much of this data is automatically generated, or not directly visible to
users during their interactions. This can create situations where, even
though users share information explicitly with services, they may be
surprised to find this data being revealed. In certain cases where the
data is legally protected, the service could be held responsible for any
leakage of sensitive information. 

How should services that need users to share data and upload files
treat additional metadata attached with files? In case of uploading
documents and images, which parts of the metadata can be treated as
explicitly shared information.

## Solution

Stripping all metadata that is not directly visible during upload time,
or during the use of the service can help protect services from
leaks and liabilities. Even in cases where the information is not
legally protected, the service can protect themselves from surprising
their users and thus alienating them. 

Additionally when users share data with services, they can be presented
with a preview of the data obtained by the service, including any
metadata ``[[Preview Shared Data]]``. This allows users to be more aware
of information that they are sharing with the services, and in many
cases with other entities on the Internet.

To summarize: user metadata that can not be made visible to users
clearly should be stripped to avoid overstepping the users' expectations. 

## Examples

#### Uploading images to twitter.com

Twitter.com removes EXIF data from images uploaded to their image
sharing service. Previously there have been many breaches of personal
location by using EXIF data shared by image sharing services. 

#### Hiding EXIF data on Flickr.com

In certain cases services might build features based on
metadata, or the metadata sharing could be an important part of the
community of users. Flickr.com allows users to hide their EXIF data from
public display, and also provides an interface for users to easily see
whether they are sharing location as part of uploading their images. 

_TODO: add screenshots_


