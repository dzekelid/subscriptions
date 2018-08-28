{
  "info": {
    "name": "Amazon RDS API Describe Event Subscriptions",
    "_postman_id": "97f32728-b91d-4c77-a331-9b4b37604386",
    "description": "Lists all the subscription descriptions for a customer account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "9ea26765-fe33-4669-b109-6e08751bb87c",
          "name": "addroletodbcluster",
          "request": {
            "url": "http://example.com/api/?Action=AddRoleToDBCluster?DBClusterIdentifier=DBClusterIdentifier&RoleArn=RoleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates an Identity and Access Management (IAM) role from an Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "501c5739-5f36-437f-a069-83ff24130309"
            }
          ]
        },
        {
          "id": "f307cc4e-b98c-4242-ae1b-e1c507a98224",
          "name": "createdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBCluster?AvailabilityZones.AvailabilityZone.N=AvailabilityZones.AvailabilityZone.N&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&DatabaseName=DatabaseName&DBClusterIdentifier=DBClusterIdentifier&DBClusterParameterGroupName=DBClusterParameterGroupName&DBSubnetGroupName=DBSubnetGroupName&Engine=Engine&EngineVersion=EngineVersion&KmsKeyId=KmsKeyId&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&ReplicationSourceIdentifier=ReplicationSourceIdentifier&StorageEncrypted=StorageEncrypted&Tags.Tag.N=Tags.Tag.N&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97210733-109d-4bd3-9233-f23bce6e4750"
            }
          ]
        },
        {
          "id": "270e20f8-6dde-4ec9-9369-b116df81ea57",
          "name": "deletedbcluster",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBCluster?DBClusterIdentifier=DBClusterIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBCluster action deletes a previously provisioned DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8374213-a4e2-424a-974c-58539e9b93f1"
            }
          ]
        },
        {
          "id": "5c640214-47a4-4ede-bec4-3c6e9b6d6ed9",
          "name": "describedbclusters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusters?DBClusterIdentifier=DBClusterIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about provisioned Aurora DB clusters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7af6ac8-2e0d-4c73-a95d-016c462c00cd"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "6a900c1a-d98e-4168-80f3-f1c053021d9b",
          "name": "addsourceidentifiertosubscription",
          "request": {
            "url": "http://example.com/api/?Action=AddSourceIdentifierToSubscription?SourceIdentifier=SourceIdentifier&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a source identifier to an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "052df91c-6da4-4db6-aa10-2f2ed5609b2c"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "a8395df3-76dc-426e-bc31-7f8984e21dab",
          "name": "addtagstoresource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceName=ResourceName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds metadata tags to an Amazon RDS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fb684b7-e964-4b15-9bec-898e4eb5631f"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance Actions",
      "item": [
        {
          "id": "7000bd96-7d2a-4f04-a809-676f1b6f4464",
          "name": "applypendingmaintenanceaction",
          "request": {
            "url": "http://example.com/api/?Action=ApplyPendingMaintenanceAction?ApplyAction=ApplyAction&OptInType=OptInType&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a pending maintenance action to a resource (for example, to a DB instance)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c1195ee-3d8a-4eed-8e46-9bee132a098e"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Groups",
      "item": [
        {
          "id": "4ad69420-b34c-4459-8dbb-8d649bb9dd8e",
          "name": "authorizedbsecuritygroupingress",
          "request": {
            "url": "http://example.com/api/?Action=AuthorizeDBSecurityGroupIngress?CIDRIP=CIDRIP&DBSecurityGroupName=DBSecurityGroupName&EC2SecurityGroupId=EC2SecurityGroupId&EC2SecurityGroupName=EC2SecurityGroupName&EC2SecurityGroupOwnerId=EC2SecurityGroupOwnerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables ingress to a DBSecurityGroup using one of two forms of authorization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9baecde1-8930-4278-bc2a-c816e104ee54"
            }
          ]
        },
        {
          "id": "626a60e8-b69b-4658-91d6-a74894f7bbb5",
          "name": "createdbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSecurityGroup?DBSecurityGroupDescription=DBSecurityGroupDescription&DBSecurityGroupName=DBSecurityGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60c4af94-392b-4e38-8987-20fcb20d3f45"
            }
          ]
        },
        {
          "id": "af6edb8c-90ca-48d3-9150-cffa1d9fcf38",
          "name": "deletedbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSecurityGroup?DBSecurityGroupName=DBSecurityGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8a95792-d602-4d46-8a2b-a5358544122f"
            }
          ]
        },
        {
          "id": "15fa6483-d12f-4236-842f-06975570caf1",
          "name": "describedbsecuritygroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSecurityGroups?DBSecurityGroupName=DBSecurityGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBSecurityGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f88b1909-4fe6-43a2-84da-3e358f20ade2"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "27d29273-7115-447c-9d83-c2fba641e0ce",
          "name": "copydbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterParameterGroup?SourceDBClusterParameterGroupIdentifier=SourceDBClusterParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterParameterGroupDescription=TargetDBClusterParameterGroupDescription&TargetDBClusterParameterGroupIdentifier=TargetDBClusterParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da4868d8-70a7-42e3-897d-f50c10583c7d"
            }
          ]
        },
        {
          "id": "c6234f7c-639c-41bf-9b51-6e9e79698c79",
          "name": "createdbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName&DBParameterGroupFamily=DBParameterGroupFamily&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a781dc53-7c01-47d4-adb1-bcdfe6c38e22"
            }
          ]
        },
        {
          "id": "b6355b3d-e35f-43eb-a5bb-11855a70bc01",
          "name": "deletedbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "522525d3-8434-428c-9963-f7c4d344a2e9"
            }
          ]
        },
        {
          "id": "151561a7-d489-4f27-996e-b2f3268da4eb",
          "name": "describedbclusterparametergroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterParameterGroups?DBClusterParameterGroupName=DBClusterParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBClusterParameterGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04a040fb-06ad-4c2b-944b-628845096a04"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Snapshots",
      "item": [
        {
          "id": "024a1e01-4d8c-47fd-a191-b82024307d79",
          "name": "copydbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterSnapshot?SourceDBClusterSnapshotIdentifier=SourceDBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterSnapshotIdentifier=TargetDBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2634b91-7136-4049-b598-c9c86635b446"
            }
          ]
        },
        {
          "id": "f16838c8-27ed-4caa-a31c-351e77958275",
          "name": "createdbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterSnapshot?DBClusterIdentifier=DBClusterIdentifier&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f233373e-83fc-4cf0-939c-e436923822da"
            }
          ]
        },
        {
          "id": "6ec5ee74-e95b-4a5d-853b-baf50742d182",
          "name": "deletedbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterSnapshot?DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f7af39d-499e-4246-9cbe-55f58431bbf4"
            }
          ]
        },
        {
          "id": "1d26d099-2b2d-4bde-b5c7-ce59ff6f8c97",
          "name": "describedbclustersnapshotattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterSnapshotAttributes?DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB cluster snapshot attribute names and values for a manual DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6561e4c-5596-4204-aa8b-8c42aa6ee309"
            }
          ]
        },
        {
          "id": "345e33e6-af44-4e5c-8aa1-3401018cf486",
          "name": "describedbclustersnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterSnapshots?DBClusterIdentifier=DBClusterIdentifier&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&Filters.Filter.N=Filters.Filter.N&IncludePublic=IncludePublic&IncludeShared=IncludeShared&Marker=Marker&MaxRecords=MaxRecords&SnapshotType=SnapshotType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about DB cluster snapshots."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0f1076f-759a-4bf9-91f7-ca5f9448654c"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter Groups",
      "item": [
        {
          "id": "0b0a28e0-fcfe-4314-906b-1fa1849d7efc",
          "name": "copydbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBParameterGroup?SourceDBParameterGroupIdentifier=SourceDBParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBParameterGroupDescription=TargetDBParameterGroupDescription&TargetDBParameterGroupIdentifier=TargetDBParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c33d97ae-1a9b-4549-9d42-550c98b2bd6f"
            }
          ]
        },
        {
          "id": "8d8c18d3-2e17-423d-8e1e-ca14330870de",
          "name": "createdbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBParameterGroup?DBParameterGroupFamily=DBParameterGroupFamily&DBParameterGroupName=DBParameterGroupName&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a384b86-8334-4312-884f-80334a0afa25"
            }
          ]
        },
        {
          "id": "6bec2d28-77cb-440b-a2bb-2fc2101f8752",
          "name": "deletedbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBParameterGroup?DBParameterGroupName=DBParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DBParameterGroup."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "312fd275-61c3-469c-a5d1-9c235ecb1476"
            }
          ]
        },
        {
          "id": "67bebf49-ad60-46e7-8b80-65e844fa6059",
          "name": "describedbparametergroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBParameterGroups?DBParameterGroupName=DBParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBParameterGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70117906-349b-4f21-b0e8-38eb58c96d9f"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "98d81a13-a543-48c9-b5cf-5a794fd74f36",
          "name": "copydbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBSnapshot?CopyTags=CopyTags&KmsKeyId=KmsKeyId&PreSignedUrl=PreSignedUrl&SourceDBSnapshotIdentifier=SourceDBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBSnapshotIdentifier=TargetDBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "930dd6bc-e181-497d-9252-78e0e7d62124"
            }
          ]
        },
        {
          "id": "1eab0b23-fc1a-416c-a8e0-c89b4fe737de",
          "name": "createdbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSnapshot?DBInstanceIdentifier=DBInstanceIdentifier&DBSnapshotIdentifier=DBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53272ac1-9056-4ae2-98ef-673ce9f9a51b"
            }
          ]
        },
        {
          "id": "07dcbcc3-d2c5-4186-80c1-5c2514481d9e",
          "name": "deletedbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSnapshot?DBSnapshotIdentifier=DBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6dd36ce7-1dab-40b4-a2a6-5be7e6743632"
            }
          ]
        },
        {
          "id": "2363c931-7cdc-4fda-a258-d505867594c6",
          "name": "describedbsnapshotattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSnapshotAttributes?DBSnapshotIdentifier=DBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB snapshot attribute names and values for a manual DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2fb0654-dc38-4787-9340-30d1fa1ea368"
            }
          ]
        },
        {
          "id": "a72abc8f-78f9-4239-a5a0-aa6134cfdb6a",
          "name": "describedbsnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSnapshots?DBInstanceIdentifier=DBInstanceIdentifier&DBSnapshotIdentifier=DBSnapshotIdentifier&Filters.Filter.N=Filters.Filter.N&IncludePublic=IncludePublic&IncludeShared=IncludeShared&Marker=Marker&MaxRecords=MaxRecords&SnapshotType=SnapshotType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about DB snapshots."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b9531ec-5b1d-4378-ae94-d8040cb23793"
            }
          ]
        }
      ]
    },
    {
      "name": "Option Groups",
      "item": [
        {
          "id": "1772aa62-740b-4057-9a8b-2e7145dd1d49",
          "name": "copyoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyOptionGroup?SourceOptionGroupIdentifier=SourceOptionGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetOptionGroupDescription=TargetOptionGroupDescription&TargetOptionGroupIdentifier=TargetOptionGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29513fce-a0f2-4c60-aa00-ccb189ad7cbc"
            }
          ]
        },
        {
          "id": "578ede2e-7cc4-4e17-af7f-3ddd64652bd8",
          "name": "createoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateOptionGroup?EngineName=EngineName&MajorEngineVersion=MajorEngineVersion&OptionGroupDescription=OptionGroupDescription&OptionGroupName=OptionGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "861e27db-ef61-4f9f-970a-9c59dac00b00"
            }
          ]
        },
        {
          "id": "236bb721-841a-4a95-a441-03f23ae1feca",
          "name": "deleteoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteOptionGroup?OptionGroupName=OptionGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75fee3f2-15f9-488c-b141-3e041c26376e"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "2365a374-09af-4061-8b93-dcaf12b6ab1d",
          "name": "createdbinstance",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstance?AllocatedStorage=AllocatedStorage&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&CopyTagsToSnapshot=CopyTagsToSnapshot&DBClusterIdentifier=DBClusterIdentifier&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBName=DBName&DBParameterGroupName=DBParameterGroupName&DBSecurityGroups.DBSecurityGroupName.N=DBSecurityGroups.DBSecurityGroupName.N&DBSubnetGroupName=DBSubnetGroupName&Domain=Domain&DomainIAMRoleName=DomainIAMRoleName&Engine=Engine&EngineVersion=EngineVersion&Iops=Iops&KmsKeyId=KmsKeyId&LicenseModel=LicenseModel&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&MultiAZ=MultiAZ&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PromotionTier=PromotionTier&PubliclyAccessible=PubliclyAccessible&StorageEncrypted=StorageEncrypted&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N&TdeCredentialArn=TdeCredentialArn&TdeCredentialPassword=TdeCredentialPassword&Timezone=Timezone&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab30c529-c711-40db-a475-e292ed0c2f4d"
            }
          ]
        },
        {
          "id": "a7650205-7bf1-40b7-9ac9-9aa31d8d6c50",
          "name": "createdbinstancereadreplica",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstanceReadReplica?AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&CopyTagsToSnapshot=CopyTagsToSnapshot&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBSubnetGroupName=DBSubnetGroupName&Iops=Iops&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&OptionGroupName=OptionGroupName&Port=Port&PubliclyAccessible=PubliclyAccessible&SourceDBInstanceIdentifier=SourceDBInstanceIdentifier&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DB instance for a DB instance running MySQL, MariaDB, or PostgreSQL that acts as a Read Replica of a source DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e4dae2f-b20f-4bae-ba59-226b8921bd80"
            }
          ]
        },
        {
          "id": "53cc38bf-f035-4102-9763-0bfb395c61c0",
          "name": "deletedbinstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBInstance?DBInstanceIdentifier=DBInstanceIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBInstance action deletes a previously provisioned DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd72b830-0fb9-429b-8e2b-1a16adb47710"
            }
          ]
        },
        {
          "id": "28fda99c-9791-4c3f-98e5-9386332423ab",
          "name": "describedbinstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBInstances?DBInstanceIdentifier=DBInstanceIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about provisioned RDS instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "970ee77a-6aba-4f05-a4f3-a969100774ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Subnet Groups",
      "item": [
        {
          "id": "878bba74-4d0c-47cc-a514-d056584eac2b",
          "name": "createdbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSubnetGroup?DBSubnetGroupDescription=DBSubnetGroupDescription&DBSubnetGroupName=DBSubnetGroupName&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e74a8912-4583-4664-afb2-cacee711a4e0"
            }
          ]
        },
        {
          "id": "a304d8a2-3c58-4614-8cd7-e6aedf1c3e07",
          "name": "deletedbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSubnetGroup?DBSubnetGroupName=DBSubnetGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6776648e-9b3e-4583-8cf6-67e639b7de1d"
            }
          ]
        },
        {
          "id": "97e98ff5-1da7-4ef2-aabc-60ba53d32061",
          "name": "describedbsubnetgroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBSubnetGroups?DBSubnetGroupName=DBSubnetGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DBSubnetGroup descriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ee10e88-a54b-495d-9f84-7acedb8e578f"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "554887fa-6552-4c8c-8a85-94ba8baebacf",
          "name": "createeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=CreateEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&SnsTopicArn=SnsTopicArn&SourceIds.SourceId.N=SourceIds.SourceId.N&SourceType=SourceType&SubscriptionName=SubscriptionName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a15b24b-b027-4723-b5ec-35938a7f1082"
            }
          ]
        },
        {
          "id": "df8c1951-e393-4e81-a522-b537c577af72",
          "name": "deleteeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEventSubscription?SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c1e714a-15c1-47c8-8325-9ce3bffd58bf"
            }
          ]
        },
        {
          "id": "026f163c-85d8-44fc-912d-97bf45ed7dc4",
          "name": "describeeventsubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventSubscriptions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the subscription descriptions for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "056754e0-a233-40cb-b6a5-6d7d517ae669"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "5eb81c63-cc71-48c3-85c7-7c1e5db05d3e",
          "name": "describeaccountattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountAttributes?AccountQuotas.AccountQuota.N=AccountQuotas.AccountQuota.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the attributes for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6107ce1-b9a1-43fc-bc60-3dc4f2b19d9e"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "2294238a-8bf1-4522-817a-23457258418b",
          "name": "describecertificates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCertificates?CertificateIdentifier=CertificateIdentifier&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the set of CA certificates provided by Amazon RDS for this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b30487b-9c6e-4036-becb-d78de9c5f223"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameters",
      "item": [
        {
          "id": "1bbdbd1d-cf79-47db-ad7f-b3aece7b8331",
          "name": "describedbclusterparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBClusterParameters?DBClusterParameterGroupName=DBClusterParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&Source=Source",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed parameter list for a particular DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0befd07-84ab-4356-a821-817a5991446e"
            }
          ]
        }
      ]
    },
    {
      "name": "Engines",
      "item": [
        {
          "id": "796c1312-f44f-4a66-8db8-8502b4fb2ab7",
          "name": "describedbengineversions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBEngineVersions?DBParameterGroupFamily=DBParameterGroupFamily&DefaultOnly=DefaultOnly&Engine=Engine&EngineVersion=EngineVersion&Filters.Filter.N=Filters.Filter.N&ListSupportedCharacterSets=ListSupportedCharacterSets&ListSupportedTimezones=ListSupportedTimezones&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available DB engines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9bf124c-d0cb-45a4-a35e-ab0a8eeb0f45"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog Files",
      "item": [
        {
          "id": "ac15701b-557e-4342-b1f7-2d68f239a026",
          "name": "describedblogfiles",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBLogFiles?DBInstanceIdentifier=DBInstanceIdentifier&FileLastWritten=FileLastWritten&FilenameContains=FilenameContains&FileSize=FileSize&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of DB log files for the DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "260f75ec-38bd-402a-b0f3-d2b20da62efa"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "e5081844-d7fc-46bf-8df4-25e7f2a1cde7",
          "name": "describedbparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDBParameters?DBParameterGroupName=DBParameterGroupName&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&Source=Source",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the detailed parameter list for a particular DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5fb2c583-201c-4a71-9c61-664d312eaa9d"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Cluster Parameters",
      "item": [
        {
          "id": "f9d45367-b0ca-4584-a14e-1d7f2a78aebb",
          "name": "describeenginedefaultclusterparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEngineDefaultClusterParameters?DBParameterGroupFamily=DBParameterGroupFamily&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default engine and system parameter information for the cluster database engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abf9c50c-cba6-4607-8ea6-30868fca8100"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Parameters",
      "item": [
        {
          "id": "598de1ec-c1fe-4cf1-a12d-348f94f89ee2",
          "name": "describeenginedefaultparameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEngineDefaultParameters?DBParameterGroupFamily=DBParameterGroupFamily&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the default engine and system parameter information for the specified database engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40e0f489-8c93-4d29-bcdd-a337c51ff75f"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Categories",
      "item": [
        {
          "id": "4fda034f-fd9f-4531-8518-b8b904e2c3a5",
          "name": "describeeventcategories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventCategories?Filters.Filter.N=Filters.Filter.N&SourceType=SourceType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Displays a list of categories for all event source types, or, if specified, for a specified source type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee9339a1-7e1b-4cf7-b7c7-7901228c3777"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "018a4358-4479-42b4-a1d9-525cf450aee9",
          "name": "describeevents",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEvents?Duration=Duration&EndTime=EndTime&EventCategories.EventCategory.N=EventCategories.EventCategory.N&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&SourceIdentifier=SourceIdentifier&SourceType=SourceType&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns events related to DB instances, DB security groups, DB snapshots, and DB parameter groups for the past 14 days."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "195d8f0b-aa70-499d-88f3-827b6917fa0a"
            }
          ]
        }
      ]
    }
  ]
}