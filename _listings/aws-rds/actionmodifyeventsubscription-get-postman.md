{
  "info": {
    "name": "Amazon RDS API Modify Event Subscription",
    "_postman_id": "a8117d06-e68c-49b0-bd2e-899b19563c8c",
    "description": "Modifies an existing RDS event notification subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "d20dc813-3c15-40f9-82e3-cb6b3add2c1d",
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
              "id": "8669acd0-8a26-470e-b0e1-7749da57fe39"
            }
          ]
        },
        {
          "id": "e5b5e0c2-8075-4899-90e8-af039d3c1d57",
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
              "id": "2875b8f4-e506-477f-8af6-8cf10f4b662d"
            }
          ]
        },
        {
          "id": "49711f40-ba7f-4aec-9f8a-371899853f6f",
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
              "id": "6a307d2d-3cfa-4fb9-932e-a827b8d29423"
            }
          ]
        },
        {
          "id": "78b75529-a3a2-49cf-bfba-0337ea639602",
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
              "id": "22310dcf-2a6f-427e-984a-c57eb835ddec"
            }
          ]
        },
        {
          "id": "b0b72e58-2e8a-450c-8dd8-b52151df0fa0",
          "name": "failoverdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=FailoverDBCluster?DBClusterIdentifier=DBClusterIdentifier&TargetDBInstanceIdentifier=TargetDBInstanceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forces a failover for a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2caf4e7c-125a-4538-b35e-1f5557ac0e57"
            }
          ]
        },
        {
          "id": "67ac4355-2079-4757-b79e-a553c4aaa4e2",
          "name": "modifydbcluster",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBCluster?ApplyImmediately=ApplyImmediately&BackupRetentionPeriod=BackupRetentionPeriod&DBClusterIdentifier=DBClusterIdentifier&DBClusterParameterGroupName=DBClusterParameterGroupName&MasterUserPassword=MasterUserPassword&NewDBClusterIdentifier=NewDBClusterIdentifier&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modify a setting for an Amazon Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9784e927-0057-4feb-86bd-779e0560cf2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "bd954322-0975-4426-9819-58d5c5c053b7",
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
              "id": "05d7094e-bfee-48e6-af4b-f5b82a52ec26"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "030afc4d-f149-418e-a3b6-1ad2e1b0191f",
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
              "id": "58bdf4be-7b50-4035-adfa-61ddf6cb0158"
            }
          ]
        },
        {
          "id": "3b2ec6f2-eb5b-43c8-a2a8-c41b873b20c1",
          "name": "listtagsforresource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?Filters.Filter.N=Filters.Filter.N&ResourceName=ResourceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags on an Amazon RDS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef8dd965-9107-4471-84c3-c11ec133ce06"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance Actions",
      "item": [
        {
          "id": "0bd511a0-22c5-4c93-8599-0ab5e27f136f",
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
              "id": "d54553cf-6c89-4f66-9ebf-f0742771140a"
            }
          ]
        },
        {
          "id": "49bac74b-f34c-4990-9cf5-eb2dcee1d150",
          "name": "describependingmaintenanceactions",
          "request": {
            "url": "http://example.com/api/?Action=DescribePendingMaintenanceActions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of resources (for example, DB instances) that have at least one pending maintenance action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63d2da06-2db3-4d95-9aed-2d62b1c25fc2"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Groups",
      "item": [
        {
          "id": "6cdd0a96-c6b2-4ad8-a7f7-3d6181f95cc3",
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
              "id": "7dd4afab-97f4-4dc1-b675-56eec019ea2d"
            }
          ]
        },
        {
          "id": "1cb5ee2c-2a6a-4ae5-a1cd-222c1091dab5",
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
              "id": "1b494a62-0074-4017-9f22-41341220069b"
            }
          ]
        },
        {
          "id": "34d069dc-00ca-494b-89f4-20701342031e",
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
              "id": "832d1632-9aca-43d5-9047-a41f8330a9a1"
            }
          ]
        },
        {
          "id": "f400a35c-14fc-4046-9081-526403b81b1b",
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
              "id": "ba3d9fc0-b2bd-4131-aa6f-9ea50d6ffee5"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "21ec709e-af75-4259-bba0-caeadd21ca8c",
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
              "id": "dd07d02f-8c2f-417e-b98e-ae76cb117588"
            }
          ]
        },
        {
          "id": "08c5c798-bbd0-41bd-a646-921dda9114fd",
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
              "id": "ace6cedb-fb06-478c-94aa-5212bdfb767d"
            }
          ]
        },
        {
          "id": "2104d904-ae19-4231-8d40-e1c6f665003a",
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
              "id": "9e84f1c8-8d13-47d5-bfc5-e1ebc21ca811"
            }
          ]
        },
        {
          "id": "9900eafc-1083-4449-b2a4-98970fac6742",
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
              "id": "e62dcc95-e899-4b8c-b571-2fb05ba09093"
            }
          ]
        },
        {
          "id": "d20dd9ef-c3cb-48f2-bc13-49b607cc4c31",
          "name": "modifydbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName&Parameters.Parameter.N=Parameters.Parameter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the parameters of a DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60c3a64a-4524-4858-9b0a-b4995ac6ceff"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Snapshots",
      "item": [
        {
          "id": "0198a110-0d9d-4f7d-a0fd-17678903b52f",
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
              "id": "1cbece5a-c3cc-4d21-b045-6a3524e3154a"
            }
          ]
        },
        {
          "id": "e0313502-0bf7-4705-9f16-6d50d9c55f78",
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
              "id": "c902d887-32ca-4ddb-a2c2-8f1210e1bfbd"
            }
          ]
        },
        {
          "id": "f730cdff-d170-4b0e-b033-265d34e3844b",
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
              "id": "2b3d314e-e8cd-4f0c-9645-02ed8eec567c"
            }
          ]
        },
        {
          "id": "9b4b36a5-cb8c-4872-9a7b-6f2886e3e01e",
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
              "id": "75121b26-87cc-471d-8218-3cea37ab860e"
            }
          ]
        },
        {
          "id": "cca39d06-2fd4-4617-a2cf-1a29ed45daf1",
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
              "id": "52056523-dbe6-453c-9d7f-b3aafa66b525"
            }
          ]
        },
        {
          "id": "779ac56a-58dc-440e-bc81-fe1cd1e9a32b",
          "name": "modifydbclustersnapshotattribute",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBClusterSnapshotAttribute?AttributeName=AttributeName&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&ValuesToAdd.AttributeValue.N=ValuesToAdd.AttributeValue.N&ValuesToRemove.AttributeValue.N=ValuesToRemove.AttributeValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an attribute and values to, or removes an attribute and values from, a manual DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa8715ab-5d87-40bb-88b1-23dae2eb9e1d"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter Groups",
      "item": [
        {
          "id": "0778ed8e-b0f4-4daf-864b-c3d55940902c",
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
              "id": "59786274-e499-49d7-b38d-93057e740e9b"
            }
          ]
        },
        {
          "id": "2af9cbb3-e0d7-4ba0-b162-b86a07a9416d",
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
              "id": "58c72310-e40b-4e1b-bff1-6fdc9d0d1c5a"
            }
          ]
        },
        {
          "id": "7f359b96-209c-4f9d-93af-5cede044bd3d",
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
              "id": "a4e72e14-a8dd-47c3-a31c-b9aef939cbcd"
            }
          ]
        },
        {
          "id": "5bd2e60d-1525-4a7d-a1ea-8eafe7df1798",
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
              "id": "fabcd875-2290-4f87-93c9-df1e719af2ba"
            }
          ]
        },
        {
          "id": "6a7cf6b3-9c18-43db-8f7a-6e57e43ccfb6",
          "name": "modifydbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBParameterGroup?DBParameterGroupName=DBParameterGroupName&Parameters.Parameter.N=Parameters.Parameter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the parameters of a DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d1a96c8-9b6b-4902-80a9-8fb68dcca29c"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "d42fdb92-6d58-4ec7-92b9-eb9062cffb39",
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
              "id": "48d165bf-a38f-475b-bfdd-75ec085844ec"
            }
          ]
        },
        {
          "id": "60891784-51d9-456e-97b5-accbbe7af0fb",
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
              "id": "d59d0a85-2cc4-4cf8-b521-3959a6b83913"
            }
          ]
        },
        {
          "id": "d8686a2f-9e5c-4176-8d83-095e03fc8050",
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
              "id": "bf9bc96d-bddc-447a-a30b-50eabe92369e"
            }
          ]
        },
        {
          "id": "83f4673d-2498-4045-87ed-b5c06331e8c9",
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
              "id": "1102f185-5358-49c5-858a-1fa442dff6ba"
            }
          ]
        },
        {
          "id": "121a206f-efb8-4356-a443-f04a53d3a022",
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
              "id": "277566cf-a153-417f-8221-16f33b6f3590"
            }
          ]
        },
        {
          "id": "c638cd79-e4cd-46ea-b4f9-b348de6cad0e",
          "name": "modifydbsnapshotattribute",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBSnapshotAttribute?AttributeName=AttributeName&DBSnapshotIdentifier=DBSnapshotIdentifier&ValuesToAdd.AttributeValue.N=ValuesToAdd.AttributeValue.N&ValuesToRemove.AttributeValue.N=ValuesToRemove.AttributeValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an attribute and values to, or removes an attribute and values from, a manual DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3adc3d4b-d234-4e50-a568-6efe2d501354"
            }
          ]
        }
      ]
    },
    {
      "name": "Option Groups",
      "item": [
        {
          "id": "a829e205-1400-4f9f-956b-577b6f326796",
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
              "id": "1881d2a0-d615-4971-a850-d073b8a48c4b"
            }
          ]
        },
        {
          "id": "51c39968-6bcc-4ae3-b052-54b60228bb5b",
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
              "id": "545fcf4e-8621-4765-a4f4-cd95a5a4db60"
            }
          ]
        },
        {
          "id": "cba6ab2b-7bb5-4e3e-83c7-ae9c5b680101",
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
              "id": "061ac4bd-c3de-4f40-8015-98c50581b157"
            }
          ]
        },
        {
          "id": "b4c7014b-f0c3-4b82-80aa-08ac11638ecc",
          "name": "describeoptiongroupoptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOptionGroupOptions?EngineName=EngineName&Filters.Filter.N=Filters.Filter.N&MajorEngineVersion=MajorEngineVersion&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes all available options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4ef96e5-4c67-4f4b-9c11-372a205503e4"
            }
          ]
        },
        {
          "id": "37b225e1-0ace-416e-a4bd-00450b511fd2",
          "name": "describeoptiongroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOptionGroups?EngineName=EngineName&Filters.Filter.N=Filters.Filter.N&MajorEngineVersion=MajorEngineVersion&Marker=Marker&MaxRecords=MaxRecords&OptionGroupName=OptionGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available option groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "890b7bed-2776-40c9-ad96-6d64b36f7795"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "997d006b-fbec-4d0e-8343-d56dd77a947b",
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
              "id": "41d1129f-bfbb-4806-9d59-4b97e475e9d8"
            }
          ]
        },
        {
          "id": "4ca4c322-7585-4d06-97e8-d661fc0f437b",
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
              "id": "9ec9d4ff-8cff-4101-9000-4885686d5b02"
            }
          ]
        },
        {
          "id": "92c9bc2f-9401-45e7-88cc-c8e04f350fe3",
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
              "id": "b41a26f5-f6df-48fe-a6c0-f8d5760fa621"
            }
          ]
        },
        {
          "id": "638012eb-dcdd-4f60-89e4-bf96c854b2d9",
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
              "id": "81cda133-cbf0-447f-a31a-3ec0724d2eab"
            }
          ]
        },
        {
          "id": "cf3c1404-e908-4cc1-a21a-c3b850998b42",
          "name": "describeorderabledbinstanceoptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOrderableDBInstanceOptions?DBInstanceClass=DBInstanceClass&Engine=Engine&EngineVersion=EngineVersion&Filters.Filter.N=Filters.Filter.N&LicenseModel=LicenseModel&Marker=Marker&MaxRecords=MaxRecords&Vpc=Vpc",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of orderable DB instance options for the specified engine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f9dd039-3ca8-43de-8509-82168388d292"
            }
          ]
        },
        {
          "id": "4dfc20ec-6ac4-4d81-9f79-e7f44b509d83",
          "name": "describereserveddbinstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedDBInstances?DBInstanceClass=DBInstanceClass&Duration=Duration&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&MultiAZ=MultiAZ&OfferingType=OfferingType&ProductDescription=ProductDescription&ReservedDBInstanceId=ReservedDBInstanceId&ReservedDBInstancesOfferingId=ReservedDBInstancesOfferingId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about reserved DB instances for this account, or about a specified reserved DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4358c6fb-0e04-4dbb-93fd-ee3fec3ab5f1"
            }
          ]
        },
        {
          "id": "010f938d-7fec-4da4-8f08-d1d2fce98987",
          "name": "describereserveddbinstancesofferings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedDBInstancesOfferings?DBInstanceClass=DBInstanceClass&Duration=Duration&Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&MultiAZ=MultiAZ&OfferingType=OfferingType&ProductDescription=ProductDescription&ReservedDBInstancesOfferingId=ReservedDBInstancesOfferingId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists available reserved DB instance offerings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb178eb5-60bb-4cc7-a2d8-df44c28d4792"
            }
          ]
        },
        {
          "id": "374a6d36-ec83-499f-b4cd-4432207d6e17",
          "name": "modifydbinstance",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBInstance?AllocatedStorage=AllocatedStorage&AllowMajorVersionUpgrade=AllowMajorVersionUpgrade&ApplyImmediately=ApplyImmediately&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&BackupRetentionPeriod=BackupRetentionPeriod&CACertificateIdentifier=CACertificateIdentifier&CopyTagsToSnapshot=CopyTagsToSnapshot&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBParameterGroupName=DBParameterGroupName&DBPortNumber=DBPortNumber&DBSecurityGroups.DBSecurityGroupName.N=DBSecurityGroups.DBSecurityGroupName.N&DBSubnetGroupName=DBSubnetGroupName&Domain=Domain&DomainIAMRoleName=DomainIAMRoleName&EngineVersion=EngineVersion&Iops=Iops&LicenseModel=LicenseModel&MasterUserPassword=MasterUserPassword&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&MultiAZ=MultiAZ&NewDBInstanceIdentifier=NewDBInstanceIdentifier&OptionGroupName=OptionGroupName&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PromotionTier=PromotionTier&PubliclyAccessible=PubliclyAccessible&StorageType=StorageType&TdeCredentialArn=TdeCredentialArn&TdeCredentialPassword=TdeCredentialPassword&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies settings for a DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d8c3f3a-161d-457a-835f-33b887febb6d"
            }
          ]
        }
      ]
    },
    {
      "name": "Subnet Groups",
      "item": [
        {
          "id": "245b679d-9242-437e-9acb-187247f62fc4",
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
              "id": "c292b030-2694-408b-860f-ba3236c74d5c"
            }
          ]
        },
        {
          "id": "208b30cc-7b9c-4e7e-b36b-95cf3506004b",
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
              "id": "ad3b5ee4-12f8-48e6-97ad-e038fadde733"
            }
          ]
        },
        {
          "id": "95912266-efe8-480b-a041-21cf2b281c31",
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
              "id": "d5fc3a65-3a2a-4bcf-bfca-e191e04414a7"
            }
          ]
        },
        {
          "id": "bf53b71a-2a80-4caf-b89b-4dfe0ba14f3c",
          "name": "modifydbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyDBSubnetGroup?DBSubnetGroupDescription=DBSubnetGroupDescription&DBSubnetGroupName=DBSubnetGroupName&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a78493d8-6f02-4264-8e95-22962a60652f"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "92c065ae-5554-4a3d-9028-2a165a2c1367",
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
              "id": "22f8cbb8-71da-494e-b12d-bd9578016c07"
            }
          ]
        },
        {
          "id": "7b2e56cf-fb7b-484d-b164-9570b2ef3d7c",
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
              "id": "9e962eaf-a6ee-449a-b7ee-257ea0aa70d3"
            }
          ]
        },
        {
          "id": "2f8cec7f-fe22-43c5-bde0-1a95b99a35a5",
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
              "id": "2c011515-95a8-4d4b-bd4e-66bada0657ec"
            }
          ]
        },
        {
          "id": "0536c480-a34b-471d-a77f-26b2d8a9e354",
          "name": "modifyeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=ModifyEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&SnsTopicArn=SnsTopicArn&SourceType=SourceType&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "868095e9-0159-49d9-8d41-d8317fb98f3d"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "8382f5c7-e37a-405a-912e-5cd688857b0f",
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
              "id": "19b5984d-d3e2-4ca6-a899-3ccdc9aa72c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "3163ff4b-32e7-4e28-a4af-6c35f421064a",
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
              "id": "6f9ed415-efd4-445d-ab06-4f089fa8b3ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameters",
      "item": [
        {
          "id": "45de9ad8-d49c-4bcd-8a94-0064f73ae5bd",
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
              "id": "50890f7c-ed12-4495-9df8-b65d87f0bbd5"
            }
          ]
        }
      ]
    },
    {
      "name": "Engines",
      "item": [
        {
          "id": "9740662f-b317-496c-b76e-02039398f9ec",
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
              "id": "5d9cb177-2915-4977-afb2-6e6ab2f18116"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog Files",
      "item": [
        {
          "id": "26e73cd1-d55a-4bde-bdd6-16cf166042aa",
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
              "id": "b99e244a-990a-43b9-9a2e-d6b1a272d302"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "0861a996-0f42-4c72-9bb5-9624b5cc74bf",
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
              "id": "1fce849d-3a88-43db-bac0-9b2c6f487f0f"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Cluster Parameters",
      "item": [
        {
          "id": "e994cdb8-12a9-4b6d-8ab4-deda8733f4fb",
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
              "id": "e31ea22b-3fff-45fb-a119-48a0c75e889d"
            }
          ]
        }
      ]
    },
    {
      "name": "Default Parameters",
      "item": [
        {
          "id": "89c455db-c97a-42dd-8f69-35107ab6b0c5",
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
              "id": "e026c3c6-3425-4f89-b98a-deaccca77d58"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Categories",
      "item": [
        {
          "id": "30d3c1f2-4b2c-4a0a-9972-2d14f01c9eb1",
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
              "id": "92cb41f1-1397-4043-90c5-86a2f41d6155"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "472c2857-8c57-4f68-a561-6965966f1fc1",
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
              "id": "97741f50-c69b-4e21-a517-8951aeead0fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Source Regions",
      "item": [
        {
          "id": "0aca03c8-cf60-478a-bac4-e30711b52d2d",
          "name": "describesourceregions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSourceRegions?Filters.Filter.N=Filters.Filter.N&Marker=Marker&MaxRecords=MaxRecords&RegionName=RegionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the source AWS regions where the current AWS region can create a Read Replica \n            or copy a DB snapshot from."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a27e07c-1415-4dcc-884a-e05037f9aa01"
            }
          ]
        }
      ]
    },
    {
      "name": "Log Files",
      "item": [
        {
          "id": "987ac0f6-1e30-47c3-8905-d5fd9fdd5154",
          "name": "downloaddblogfileportion",
          "request": {
            "url": "http://example.com/api/?Action=DownloadDBLogFilePortion?DBInstanceIdentifier=DBInstanceIdentifier&LogFileName=LogFileName&Marker=Marker&NumberOfLines=NumberOfLines",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Downloads all or a portion of the specified log file, up to 1 MB in size."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2a2faea-2b53-46a7-bab0-031d357817f6"
            }
          ]
        }
      ]
    }
  ]
}