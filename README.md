# `flutter/flutter` Issue #96272 repro case

This project is a minimised reproduction for [flutter/flutter Issue #96272](https://github.com/flutter/flutter/issues/96272)

Building on macOS:

```console
$ dart run build_runner build --delete-conflicting-outputs 
Building package executable... (1.6s)
Built build_runner:build_runner.
[INFO] Generating build script completed, took 455ms
[INFO] Reading cached asset graph completed, took 63ms
[INFO] Checking for updates since last build completed, took 554ms
[WARNING] gql_build:serializer_builder on lib/$lib$:
Your current `analyzer` version may not fully support your current SDK version.

Analyzer language version: 2.14.0
SDK language version: 2.15.0

Please update to the latest `analyzer` version (3.0.0) by running
`flutter packages upgrade`.

If you are not getting the latest version by running the above command, you
can try adding a constraint like the following to your pubspec to start
diagnosing why you can't get the latest version:

dev_dependencies:
  analyzer: ^3.0.0 

[INFO] Running build completed, took 11.2s
[INFO] Caching finalized dependency graph completed, took 44ms
[INFO] Succeeded after 11.3s with 12 outputs (12 actions)
```

Building on Windows:
```console
PS> dart run build_runner build --delete-conflicting-outputs
[INFO] Generating build script completed, took 540ms
[INFO] Reading cached asset graph completed, took 74ms
[INFO] Checking for updates since last build completed, took 3.6s
[WARNING] gql_build:serializer_builder on lib/$lib$:
Your current `analyzer` version may not fully support your current SDK version.

Analyzer language version: 2.14.0
SDK language version: 2.15.0

Please update to the latest `analyzer` version (3.0.0) by running
`flutter packages upgrade`.

If you are not getting the latest version by running the above command, you
can try adding a constraint like the following to your pubspec to start
diagnosing why you can't get the latest version:

dev_dependencies:
  analyzer: ^3.0.0

[INFO] Running build completed, took 13.1s
[INFO] Caching finalized dependency graph completed, took 62ms
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.data.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GPullRequestsData_viewer_pullRequests_edges_node implements Built<GPullRequestsData_viewer_pullRequests_edges_node, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field url have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.        
2. Make field updatedAt have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
3. Make field state have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.data.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GPullRequestsData_viewer_pullRequests_edges_node_repository implements Built<GPullRequestsData_viewer_pullRequests_edges_node_repository, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field url have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.        
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.data.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GPullRequestsData_viewer_pullRequests_edges_node_author implements Built<GPullRequestsData_viewer_pullRequests_edges_node_author, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field url have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.        
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.data.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GAssignedIssuesData_search_edges_node__asIssue implements Built<GAssignedIssuesData_search_edges_node__asIssue, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field url have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.        
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.data.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GAssignedIssuesData_search_edges_node__asIssue_repository implements Built<GAssignedIssuesData_search_edges_node__asIssue_repository, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field url have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.        
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.data.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GAssignedIssuesData_search_edges_node__asIssue_author implements Built<GAssignedIssuesData_search_edges_node__asIssue_author, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field url have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.        
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.data.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GRepositoriesData_viewer_repositories_nodes implements Built<GRepositoriesData_viewer_repositories_nodes, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field url have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.        
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.data.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GRepositoriesData_viewer_repositories_nodes_owner implements Built<GRepositoriesData_viewer_repositories_nodes_owner, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field avatarUrl have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.req.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GViewerDetail implements Built<GViewerDetail, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field vars have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.req.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GPullRequests implements Built<GPullRequests, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field vars have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.req.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GAssignedIssues implements Built<GAssignedIssues, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field vars have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
[SEVERE] built_value_generator:built_value on lib/src/github_gql/__generated__/github_queries.req.gql.dart (cached):
Error in BuiltValueGenerator for abstract class GRepositories implements Built<GRepositories, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field vars have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GAddPullRequestReviewCommentInput implements Built<GAddPullRequestReviewCommentInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field commitOID have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GAddPullRequestReviewInput implements Built<GAddPullRequestReviewInput, dynamic>.      
Please make the following changes to use BuiltValue:

1. Make field commitOID have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field event have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GAddPullRequestReviewThreadInput implements Built<GAddPullRequestReviewThreadInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field side have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
2. Make field startSide have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GAddReactionInput implements Built<GAddReactionInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field content have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.    
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GAddVerifiableDomainInput implements Built<GAddVerifiableDomainInput, dynamic>.        
Please make the following changes to use BuiltValue:

1. Make field domain have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GAuditLogOrder implements Built<GAuditLogOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GChangeUserStatusInput implements Built<GChangeUserStatusInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field expiresAt have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCheckAnnotationData implements Built<GCheckAnnotationData, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field annotationLevel have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
2. Make field location have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.   
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCheckRunFilter implements Built<GCheckRunFilter, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field checkType have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field status have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCheckRunOutputImage implements Built<GCheckRunOutputImage, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field imageUrl have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.   
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCloneTemplateRepositoryInput implements Built<GCloneTemplateRepositoryInput, dynamic>.Please make the following changes to use BuiltValue:

1. Make field visibility have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported. 
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCommitContributionOrder implements Built<GCommitContributionOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GContributionOrder implements Built<GContributionOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCreateCheckRunInput implements Built<GCreateCheckRunInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field completedAt have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.2. Make field conclusion have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported. 
3. Make field detailsUrl have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported. 
4. Make field headSha have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.    
5. Make field output have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
6. Make field startedAt have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
7. Make field status have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCreateCheckSuiteInput implements Built<GCreateCheckSuiteInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field headSha have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.    
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCreateCommitOnBranchInput implements Built<GCreateCommitOnBranchInput, dynamic>.      
Please make the following changes to use BuiltValue:

1. Make field branch have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
2. Make field expectedHeadOid have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
3. Make field fileChanges have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.4. Make field message have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.    
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCreateDeploymentStatusInput implements Built<GCreateDeploymentStatusInput, dynamic>.  
Please make the following changes to use BuiltValue:

1. Make field state have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCreateProjectInput implements Built<GCreateProjectInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field template have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.   
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCreateRefInput implements Built<GCreateRefInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field oid have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.        
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCreateRepositoryInput implements Built<GCreateRepositoryInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field homepageUrl have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.2. Make field visibility have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported. 
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GCreateSponsorshipInput implements Built<GCreateSponsorshipInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field privacyLevel have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GDeclineTopicSuggestionInput implements Built<GDeclineTopicSuggestionInput, dynamic>.  
Please make the following changes to use BuiltValue:

1. Make field reason have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GDeploymentOrder implements Built<GDeploymentOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GDiscussionOrder implements Built<GDiscussionOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GDismissRepositoryVulnerabilityAlertInput implements Built<GDismissRepositoryVulnerabilityAlertInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field dismissReason have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GDraftPullRequestReviewThread implements Built<GDraftPullRequestReviewThread, dynamic>.Please make the following changes to use BuiltValue:

1. Make field side have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
2. Make field startSide have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GEnablePullRequestAutoMergeInput implements Built<GEnablePullRequestAutoMergeInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field mergeMethod have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GEnterpriseAdministratorInvitationOrder implements Built<GEnterpriseAdministratorInvitationOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GEnterpriseMemberOrder implements Built<GEnterpriseMemberOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GEnterpriseServerInstallationOrder implements Built<GEnterpriseServerInstallationOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GEnterpriseServerUserAccountEmailOrder implements Built<GEnterpriseServerUserAccountEmailOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GEnterpriseServerUserAccountOrder implements Built<GEnterpriseServerUserAccountOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GEnterpriseServerUserAccountsUploadOrder implements Built<GEnterpriseServerUserAccountsUploadOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GFileAddition implements Built<GFileAddition, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field contents have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.   
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GGistOrder implements Built<GGistOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GInviteEnterpriseAdminInput implements Built<GInviteEnterpriseAdminInput, dynamic>.    
Please make the following changes to use BuiltValue:

1. Make field role have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GIpAllowListEntryOrder implements Built<GIpAllowListEntryOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GIssueCommentOrder implements Built<GIssueCommentOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GIssueFilters implements Built<GIssueFilters, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field since have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GIssueOrder implements Built<GIssueOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GLabelOrder implements Built<GLabelOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GLanguageOrder implements Built<GLanguageOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GLockLockableInput implements Built<GLockLockableInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field lockReason have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported. 
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GMergePullRequestInput implements Built<GMergePullRequestInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field expectedHeadOid have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
2. Make field mergeMethod have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GMilestoneOrder implements Built<GMilestoneOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GMinimizeCommentInput implements Built<GMinimizeCommentInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field classifier have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported. 
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GOrganizationOrder implements Built<GOrganizationOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GPackageFileOrder implements Built<GPackageFileOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GPackageOrder implements Built<GPackageOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GPackageVersionOrder implements Built<GPackageVersionOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GProjectOrder implements Built<GProjectOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GPullRequestOrder implements Built<GPullRequestOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GReactionOrder implements Built<GReactionOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GRefOrder implements Built<GRefOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GRefUpdate implements Built<GRefUpdate, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field afterOid have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.   
2. Make field beforeOid have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
3. Make field name have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GReleaseOrder implements Built<GReleaseOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GRemoveReactionInput implements Built<GRemoveReactionInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field content have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.    
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GRepositoryInvitationOrder implements Built<GRepositoryInvitationOrder, dynamic>.      
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GRepositoryOrder implements Built<GRepositoryOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSavedReplyOrder implements Built<GSavedReplyOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSecurityAdvisoryIdentifierFilter implements Built<GSecurityAdvisoryIdentifierFilter, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field type have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSecurityAdvisoryOrder implements Built<GSecurityAdvisoryOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSecurityVulnerabilityOrder implements Built<GSecurityVulnerabilityOrder, dynamic>.    
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSetEnterpriseIdentityProviderInput implements Built<GSetEnterpriseIdentityProviderInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field digestMethod have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
2. Make field signatureMethod have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
3. Make field ssoUrl have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSetOrganizationInteractionLimitInput implements Built<GSetOrganizationInteractionLimitInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field expiry have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
2. Make field limit have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSetRepositoryInteractionLimitInput implements Built<GSetRepositoryInteractionLimitInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field expiry have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
2. Make field limit have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSetUserInteractionLimitInput implements Built<GSetUserInteractionLimitInput, dynamic>.Please make the following changes to use BuiltValue:

1. Make field expiry have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
2. Make field limit have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSponsorOrder implements Built<GSponsorOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSponsorableOrder implements Built<GSponsorableOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSponsorsActivityOrder implements Built<GSponsorsActivityOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSponsorsTierOrder implements Built<GSponsorsTierOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSponsorshipNewsletterOrder implements Built<GSponsorshipNewsletterOrder, dynamic>.    
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSponsorshipOrder implements Built<GSponsorshipOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GStarOrder implements Built<GStarOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GSubmitPullRequestReviewInput implements Built<GSubmitPullRequestReviewInput, dynamic>.Please make the following changes to use BuiltValue:

1. Make field event have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GTeamDiscussionCommentOrder implements Built<GTeamDiscussionCommentOrder, dynamic>.    
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GTeamDiscussionOrder implements Built<GTeamDiscussionOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GTeamMemberOrder implements Built<GTeamMemberOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GTeamOrder implements Built<GTeamOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GTeamRepositoryOrder implements Built<GTeamRepositoryOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateCheckRunInput implements Built<GUpdateCheckRunInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field completedAt have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.2. Make field conclusion have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported. 
3. Make field detailsUrl have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported. 
4. Make field output have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
5. Make field startedAt have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
6. Make field status have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.     
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseAdministratorRoleInput implements Built<GUpdateEnterpriseAdministratorRoleInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field role have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.       
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseAllowPrivateRepositoryForkingSettingInput implements Built<GUpdateEnterpriseAllowPrivateRepositoryForkingSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseDefaultRepositoryPermissionSettingInput implements Built<GUpdateEnterpriseDefaultRepositoryPermissionSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseMembersCanChangeRepositoryVisibilitySettingInput implements Built<GUpdateEnterpriseMembersCanChangeRepositoryVisibilitySettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseMembersCanCreateRepositoriesSettingInput implements Built<GUpdateEnterpriseMembersCanCreateRepositoriesSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseMembersCanDeleteIssuesSettingInput implements Built<GUpdateEnterpriseMembersCanDeleteIssuesSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseMembersCanDeleteRepositoriesSettingInput implements Built<GUpdateEnterpriseMembersCanDeleteRepositoriesSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseMembersCanInviteCollaboratorsSettingInput implements Built<GUpdateEnterpriseMembersCanInviteCollaboratorsSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseMembersCanMakePurchasesSettingInput implements Built<GUpdateEnterpriseMembersCanMakePurchasesSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseMembersCanUpdateProtectedBranchesSettingInput implements Built<GUpdateEnterpriseMembersCanUpdateProtectedBranchesSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseMembersCanViewDependencyInsightsSettingInput implements Built<GUpdateEnterpriseMembersCanViewDependencyInsightsSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseOrganizationProjectsSettingInput implements Built<GUpdateEnterpriseOrganizationProjectsSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseRepositoryProjectsSettingInput implements Built<GUpdateEnterpriseRepositoryProjectsSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseTeamDiscussionsSettingInput implements Built<GUpdateEnterpriseTeamDiscussionsSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateEnterpriseTwoFactorAuthenticationRequiredSettingInput implements Built<GUpdateEnterpriseTwoFactorAuthenticationRequiredSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateIpAllowListEnabledSettingInput implements Built<GUpdateIpAllowListEnabledSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateIpAllowListForInstalledAppsEnabledSettingInput implements Built<GUpdateIpAllowListForInstalledAppsEnabledSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateIssueInput implements Built<GUpdateIssueInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field state have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateNotificationRestrictionSettingInput implements Built<GUpdateNotificationRestrictionSettingInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field settingValue have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateProjectInput implements Built<GUpdateProjectInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field state have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdatePullRequestBranchInput implements Built<GUpdatePullRequestBranchInput, dynamic>.Please make the following changes to use BuiltValue:

1. Make field expectedHeadOid have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdatePullRequestInput implements Built<GUpdatePullRequestInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field state have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateRefInput implements Built<GUpdateRefInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field oid have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.        
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateRepositoryInput implements Built<GUpdateRepositoryInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field homepageUrl have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateSponsorshipPreferencesInput implements Built<GUpdateSponsorshipPreferencesInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field privacyLevel have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateSubscriptionInput implements Built<GUpdateSubscriptionInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field state have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUpdateTeamReviewAssignmentInput implements Built<GUpdateTeamReviewAssignmentInput, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field algorithm have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GUserStatusOrder implements Built<GUserStatusOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] built_value_generator:built_value on lib/third_party/github_graphql_schema/__generated__/schema.docs.schema.gql.dart (cached):Error in BuiltValueGenerator for abstract class GVerifiableDomainOrder implements Built<GVerifiableDomainOrder, dynamic>.
Please make the following changes to use BuiltValue:

1. Make field direction have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.  
2. Make field field have non-dynamic type. If you are already specifying a type, please make sure the type is correctly imported.      
[SEVERE] Failed after 13.5s
```