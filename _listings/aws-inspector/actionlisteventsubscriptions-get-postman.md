{
  "info": {
    "name": "AWS Inspector API List Event Subscriptions",
    "_postman_id": "2025a6c7-6dfd-463c-baa0-ca276cd84d92",
    "description": "Lists all the event subscriptions for the assessment template that is specified by\n         the ARN of the assessment template.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes To Findings",
      "item": [
        {
          "id": "39ebc885-e500-455d-a766-d36536b5f382",
          "name": "addAttributesToFindings",
          "request": {
            "url": "http://example.com/api/?Action=AddAttributesToFindings?attributes=attributes&findingArns=findingArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assigns attributes (key and value pairs) to the findings that are specified by the\n         ARNs of the findings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5fdb362-b141-4175-81b3-15704bdb2f02"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Targets",
      "item": [
        {
          "id": "f43e8c54-ecc2-456b-92b4-571084e3851d",
          "name": "createAssessmentTarget",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssessmentTarget?assessmentTargetName=assessmentTargetName&resourceGroupArn=resourceGroupArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new assessment target using the ARN of the resource group that is generated\n         by."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20b941ab-709d-4526-8f70-2a6bf609fd6a"
            }
          ]
        },
        {
          "id": "699dd067-cab4-45ad-89fd-cc78c26a7476",
          "name": "deleteAssessmentTarget",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentTarget?assessmentTargetArn=assessmentTargetArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment target that is specified by the ARN of the assessment\n         target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8e5b8b8-85d9-418a-b654-3755a6693063"
            }
          ]
        },
        {
          "id": "212b429b-416c-4cae-9d6f-5d5a920f56bb",
          "name": "describeAssessmentTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentTargets?assessmentTargetArns=assessmentTargetArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment targets that are specified by the ARNs of the assessment\n         targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49dabb78-d1ee-4475-8955-85eec94ac20c"
            }
          ]
        },
        {
          "id": "28e8618f-160c-4d57-a258-ba130caa9530",
          "name": "listAssessmentTargets",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentTargets?filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the ARNs of the assessment targets within this AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "621f35a5-7748-4ca5-ba23-690f2e7f4afe"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Templates",
      "item": [
        {
          "id": "ed826dcb-39f6-48f0-ad79-64c31e24e325",
          "name": "createAssessmentTemplate",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssessmentTemplate?assessmentTargetArn=assessmentTargetArn&assessmentTemplateName=assessmentTemplateName&durationInSeconds=durationInSeconds&rulesPackageArns=rulesPackageArns&userAttributesForFindings=userAttributesForFindings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an assessment template for the assessment target that is specified by the ARN\n         of the assessment target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9844d841-a819-4c03-9eaf-973ad2e41e2d"
            }
          ]
        },
        {
          "id": "874f035f-16a9-41ad-b1e9-7f47c7a9148a",
          "name": "deleteAssessmentTemplate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentTemplate?assessmentTemplateArn=assessmentTemplateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment template that is specified by the ARN of the assessment\n         template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "915d12ad-5640-4f6a-83b5-1e1293450481"
            }
          ]
        },
        {
          "id": "e5191c24-17de-4a02-8259-e462ae1e2f73",
          "name": "describeAssessmentTemplates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentTemplates?assessmentTemplateArns=assessmentTemplateArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment templates that are specified by the ARNs of the assessment\n         templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ec99d14-1926-41a4-b5c9-9fab05c648dd"
            }
          ]
        },
        {
          "id": "7550f3b8-09eb-48be-b786-49b105bfa7b3",
          "name": "listAssessmentTemplates",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentTemplates?assessmentTargetArns=assessmentTargetArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the assessment templates that correspond to the assessment targets that are\n         specified by the ARNs of the assessment targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df406f96-54be-465b-a6ad-724704c71642"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Groups",
      "item": [
        {
          "id": "f66d470e-97c9-4dcb-8ab0-9b32594d2698",
          "name": "createResourceGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateResourceGroup?resourceGroupTags=resourceGroupTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a resource group using the specified set of tags (key and value pairs) that\n         are used to select the EC2 instances to be included in an Amazon Inspector assessment\n         target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b89b3f5c-10de-450d-8573-d2d01cb6f293"
            }
          ]
        },
        {
          "id": "ebe25e4f-530f-482b-a344-1b84b135bc26",
          "name": "describeResourceGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeResourceGroups?resourceGroupArns=resourceGroupArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the resource groups that are specified by the ARNs of the resource\n         groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cc2f83c-152c-4f4e-9294-f7fd0b378bed"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Runs",
      "item": [
        {
          "id": "1f6332b8-8b06-4733-890e-606f74588427",
          "name": "deleteAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssessmentRun?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the assessment run that is specified by the ARN of the assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a978c772-9bf9-4de8-86ad-f893eb65054a"
            }
          ]
        },
        {
          "id": "dbee6de4-4029-40ae-8ddf-579ef1290f48",
          "name": "describeAssessmentRuns",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssessmentRuns?assessmentRunArns=assessmentRunArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the assessment runs that are specified by the ARNs of the assessment\n         runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1405b2d-8bdf-4897-bb7a-397161e85b86"
            }
          ]
        },
        {
          "id": "aeaf4e98-950d-4958-bef7-b1b415ed96dc",
          "name": "listAssessmentRuns",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentRuns?assessmentTemplateArns=assessmentTemplateArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the assessment runs that correspond to the assessment templates that are\n         specified by the ARNs of the assessment templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a740351b-d933-478c-b76f-00f62339d013"
            }
          ]
        }
      ]
    },
    {
      "name": "Cross Account Access Roles",
      "item": [
        {
          "id": "63277eb0-3087-4194-a506-2befd309f91d",
          "name": "describeCrossAccountAccessRole",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCrossAccountAccessRole?registeredAt=registeredAt&roleArn=roleArn&valid=valid",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the IAM role that enables Amazon Inspector to access your AWS\n         account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9549eeb-547b-467e-8f57-ba88cf58ce47"
            }
          ]
        }
      ]
    },
    {
      "name": "Findings",
      "item": [
        {
          "id": "f90e4d2f-26da-4d01-96e1-46c8f6ec3fa8",
          "name": "describeFindings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeFindings?findingArns=findingArns&locale=locale",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the findings that are specified by the ARNs of the findings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2b2f1f6-52b5-4e1e-b2bc-d4d5cebd8199"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules Packages",
      "item": [
        {
          "id": "8b8fd7ac-2bd9-40c6-8351-a56f602f357a",
          "name": "describeRulesPackages",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRulesPackages?locale=locale&rulesPackageArns=rulesPackageArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the rules packages that are specified by the ARNs of the rules\n         packages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee5a3a8f-39c5-47ac-a7ba-086b87b4150c"
            }
          ]
        }
      ]
    },
    {
      "name": "Telemetry Metadata",
      "item": [
        {
          "id": "b612c244-f0ab-401e-8d88-6ec8cdf566ce",
          "name": "getTelemetryMetadata",
          "request": {
            "url": "http://example.com/api/?Action=GetTelemetryMetadata?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Information about the data that is collected for the specified assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "053363d5-4c85-4c84-84c7-47021c2eea6b"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Run Agents",
      "item": [
        {
          "id": "8f3c3ee1-3c27-4b2e-b2a3-d8290a299035",
          "name": "listAssessmentRunAgents",
          "request": {
            "url": "http://example.com/api/?Action=ListAssessmentRunAgents?assessmentRunArn=assessmentRunArn&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the agents of the assessment runs that are specified by the ARNs of the\n         assessment runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a24499d3-006f-4859-b1e5-a219637d6fbb"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "b9eeb55f-3e83-43e7-bec6-ef21a27d48b0",
          "name": "listEventSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=ListEventSubscriptions?maxResults=maxResults&nextToken=nextToken&resourceArn=resourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the event subscriptions for the assessment template that is specified by\n         the ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18ada518-e311-4370-8687-bbff0b0fc397"
            }
          ]
        }
      ]
    }
  ]
}