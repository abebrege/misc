# Swagger Documentation TODO list

## Need to update
### Application | /api/application
- /lenderUser/current
- /applicantUser/current
- /
- /:applicationId/submit
- /:applicationId/programOffice/updateStatus
- /:applicationId/wfTemplate/:wfTemplateId/wfNode/next
- /:applicationId/content/upsert
- /:applicationId/content/zip-code/group/upsert
- /:applicationId/document/upsert
- /:applicationId/dataPoint/:applicationTemplateDataPointId/document/createMany
- /document/:applicationDocumentId
- /programOffice/stats

### Award | /api/award
- /
- /lenderUser/current
- /:awardId/awardStory
- /:awardId/awardStory/upsert
- /awardStory/:awardStoryId/status

### BoardMeeting | /api/boardMeeting
- /:boardMeetingId/updateWorkflowDocReviewed

### Lender | /api/lender
- /
- /:lenderId/applicationLender
- /applicationLender/:applicationLenderId
- /upsert
- /upsert/lenderUser/:lenderId
- /reactivate/lender/:lenderId/lenderUser/:lenderUserId
- /deactivate/lender/:lenderId/lenderUser/:lenderUserId
- /lenderApplications
- /user/role/lender
- /primaryContact/applicationLender/:applicationLenderId

### WorkFlow | /api/workflow 
- /wfAuditTrail/:wfInstanceId
- /wfInstance
- /WFRACI/application/:applicationId
- /WFRACI/:wfRACIId
- /WFRACI
- /wfTemplate/:wfTemplateId
- /:wfEventFlowId
- /wfInstance/application/:applicationId/boardVote/finalize
- /application/:applicationId/approval/finalize


## TODO
### Auth | /api/auth
- /deactivateUser/:userId
- /reactivateUser/:userId
- /signin
- /update/:userId/:key
- /forgot
- /user
- /update-password/:userId
- /createUser
- /verify/:userId/:key
- /setup-mfa
- /verify-mfa
- /isUserLoggedIn
- /refreshToken

### CreditAnalysis | /api/creditAnalysis
- /application/:applicationId
- /
- /:creditAnalysisId
- /creditAnalysisDataPoint/upsert
- /creditAnalysisDataPoint/:creditAnalysisDataPointId

### File | /api/file
- /ref/:File_Ref/download
- /application/:applicationId/pdf
- /awardLetter/:awardId/pdf
- /boardMemo/:boardMemoId/pdf
- /report/excelTable

### LenderApplicationNote | /api/lenderApplicationNote
- /author
- /:applicationId/upsert
- /:lenderApplicationNoteId

### OrganizationUser | /api/organizationUser
- /
- /:organizationId/:userId

### Permission | /api/permission
- /
- /access
- /groupOverrideAccess/upsert


### Todo | /api/todo
- /:userId
- /deleteMany
- /:todoId

### User | /api/user
- /
- /:roleIds
- /:userId
- /update/:userId
- /upsertUser/:userId?

