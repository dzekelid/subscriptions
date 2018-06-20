{
  "info": {
    "name": "Amazon RDS API Create Event Subscription",
    "_postman_id": "e5df4d93-0213-4ec1-a91f-3d5464611daf",
    "description": "Creates an RDS event notification subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "6043581a-a2a2-42a1-a34e-6811b07bb2af",
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
              "id": "31ef6b01-1ddc-4eb0-9dd9-405c4360d5a4"
            }
          ]
        },
        {
          "id": "43bd7426-e804-48ba-b864-d1d1bbc27dd3",
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
              "id": "9ab8aaea-9c97-4e5d-b6a4-f4dc09378438"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "332f4c13-816b-4c36-b5c3-8e763a3aa711",
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
              "id": "1a0af634-425b-4955-91d6-2a9771774ff3"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "a876399d-d479-4e1a-92bb-d89f1ccc1c79",
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
              "id": "7e88ec27-72f3-4538-a4eb-c24c0e00dcf2"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance Actions",
      "item": [
        {
          "id": "36c61e66-90df-48b7-ba7b-3704925f9679",
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
              "id": "21258993-9323-40da-9d9e-5f9e4e2df31c"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Groups",
      "item": [
        {
          "id": "494a889b-e76f-43df-9487-2628b0e3fd09",
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
              "id": "f0f21623-6f3c-4160-b8d3-5f56fea078ea"
            }
          ]
        },
        {
          "id": "562365c1-1181-406c-9adb-b76aaed01f2c",
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
              "id": "c8cc6aa9-82b7-4c01-9a05-790bf35598aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "89264e16-dde9-4b8b-891e-8bb2befe9fc7",
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
              "id": "048f056b-1f85-43e2-8439-ef3f12d3fefb"
            }
          ]
        },
        {
          "id": "9ce25dc3-8e9b-493e-af5b-2871a0a83de3",
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
              "id": "00b3e1af-9d5f-4919-b9a6-015779dcd448"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Snapshots",
      "item": [
        {
          "id": "29296280-4d41-434a-b85c-080a46b41cee",
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
              "id": "24f15d3f-f650-4cd1-89e8-0ab656497812"
            }
          ]
        },
        {
          "id": "00f62431-9cf3-4cbb-b4db-36e00cae595e",
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
              "id": "70cfade6-9604-4ec3-b617-e8c89c1848a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter Groups",
      "item": [
        {
          "id": "e19de0c5-9e75-4f32-92a0-da395c7e3fa2",
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
              "id": "c6c2196f-c9b7-45f8-9c19-a260bbfa1464"
            }
          ]
        },
        {
          "id": "7cc53130-b213-49a0-a7e8-5ad3fb1c1f2e",
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
              "id": "2747a8c6-7d0d-4ad1-8aed-218f089b3d56"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "409eb59e-0595-4246-8134-a74bb676db20",
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
              "id": "09cf37c1-edc8-47b5-a15b-6cc7e0b670c4"
            }
          ]
        },
        {
          "id": "503d138e-74de-4ca0-b77c-312e504a73a4",
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
              "id": "e3f0aa0d-2e4a-4e44-abee-4a3c4cbb5eea"
            }
          ]
        }
      ]
    },
    {
      "name": "Option Groups",
      "item": [
        {
          "id": "b9043a52-a093-4322-8a67-a45fa52606d8",
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
              "id": "4e7311d7-4abc-4dda-9a7d-2e11b7cdd121"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "1fa119a8-ac96-40bd-bf90-1fadbd95e069",
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
              "id": "8e8e31fe-3090-4dbc-b1e4-4604c0dc2820"
            }
          ]
        },
        {
          "id": "ceae2b8f-e9bf-4f7c-984a-9fd18d7b4a08",
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
              "id": "0e636744-f439-420a-b443-2cd8fa43d75a"
            }
          ]
        }
      ]
    },
    {
      "name": "Subnet Groups",
      "item": [
        {
          "id": "5aad6a57-eb7c-4674-9d1f-cab3365046ee",
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
              "id": "7fcee70b-aa31-47b1-ba1f-67e827fbfc91"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "5eb13b84-7a08-40fc-b0b0-5fb65adb6ca1",
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
              "id": "79a1c548-df81-4baa-9e94-d1c1164be6f3"
            }
          ]
        }
      ]
    }
  ]
}