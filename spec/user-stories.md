## Functional Stories

### Use Case 1: Large HTTP uploads

As a `user` and/or a `software developer`,
I want to upload large files that may or may/not complete due to network and/or server issues.  Further, for very large uploads also knowing what percentage of a file(s) that is uploaded is handy to have as both user and developer.

#### Preconditions:

User/developer is working with large files.

#### Trigger:

User attempts to upload a file.

#### Actors:

 - User with a large file
 - the server to which the file needs to be uploaded to

#### Distinction:

N/A

#### Scenario:

Large file(s) is correctly uploaded and user knows how long it was going to take within a reasonably degree of accuracy.

#### Alternative case(s):

If large file handling is not available user/developer can get notification to the lack of this particular service or an alternate unspecified method for these sizes of files.

#### Error scenario:

 - network crash and/or interruption
 - server crash and/or interruption
 - any interference that would disrupt the transfer of the large file(s) (ie cat on keyboard)
 
#### Acceptance Criteria:

User/developer has at least one methodology that will be available in order to upload (or resume) a large file(s) upload.

#### References:

- [Resumable Uploads for HTTP](https://www.ietf.org/archive/id/draft-ietf-httpbis-resumable-upload-01.html)


## Non-Functional Stories

## Technical Stories

## Spike Stories

