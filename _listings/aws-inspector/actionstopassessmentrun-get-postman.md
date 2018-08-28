{
  "info": {
    "name": "AWS Inspector API Stop Assessment Run",
    "_postman_id": "3ed0e5b1-487f-43b3-8960-d26201988c27",
    "description": "Stops the assessment run that is specified by the ARN of the assessment\n         run.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes To Findings",
      "item": [
        {
          "id": "e6fa4b0d-0bac-456b-9cf9-e106e0c07026",
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
              "id": "186e6c0e-5435-45c3-b0ba-056159aa6056"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Targets",
      "item": [
        {
          "id": "fa84c08c-4fc0-4f0c-a954-aaeea2d6d79e",
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
              "id": "220affa4-47fe-4042-bd55-8a07aacb6835"
            }
          ]
        },
        {
          "id": "81f6f765-2793-4be7-95a9-87a6b7341a90",
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
              "id": "58d13c34-b32c-4c74-bb04-d4b307ec7de4"
            }
          ]
        },
        {
          "id": "72ebbf76-ccec-46ef-bf85-5fdfbe0ec61a",
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
              "id": "c4f8f41b-9d87-471f-9cc8-9582e4c67c81"
            }
          ]
        },
        {
          "id": "847af325-62e2-4591-bae3-e2ffb0dbefd4",
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
              "id": "1c5a4f67-2867-4579-9094-4ef11d423ad3"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Templates",
      "item": [
        {
          "id": "68c303c9-6c30-4f6c-85ed-21a629105cb0",
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
              "id": "7e9f8cc5-3366-4056-8544-08745be2c305"
            }
          ]
        },
        {
          "id": "21a3a8d1-1be3-4f3d-a51a-401188b1f9fa",
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
              "id": "812f242e-5766-4ab6-bb27-51bf4db520a7"
            }
          ]
        },
        {
          "id": "b4bbd480-b32d-44b5-9de2-df00c9319601",
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
              "id": "5524e444-c828-46d1-af37-2b25e82565fd"
            }
          ]
        },
        {
          "id": "a7fcda21-97cc-44c2-821b-e9d4ffa54f66",
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
              "id": "a639df5a-8b3c-49bb-99d0-9a3d5e2cde34"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Groups",
      "item": [
        {
          "id": "a559c31d-57c1-41e6-a16b-f67fa7cf5da4",
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
              "id": "ddb514d5-1594-4518-9582-c4db040c4b11"
            }
          ]
        },
        {
          "id": "7680aeee-8642-4e49-9857-9e452149a3f8",
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
              "id": "75bfacb2-0f2f-46ca-82ea-50a9df43e51f"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Runs",
      "item": [
        {
          "id": "8f6de018-01d8-498d-91c6-e61c64e64162",
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
              "id": "eb530fd6-726e-473d-a6d8-d030a7f5c2fa"
            }
          ]
        },
        {
          "id": "24c493ea-09d0-4e9a-ac44-4e45232e2c29",
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
              "id": "b557c9e7-ea31-4393-9275-5ca18a45986d"
            }
          ]
        },
        {
          "id": "627ffe95-583f-4ee4-af7d-ac0d9447abdd",
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
              "id": "d21a24a4-689c-4551-a256-94ebe8d209e0"
            }
          ]
        },
        {
          "id": "18002e20-bab6-4d73-b1b0-90e00bdb78e4",
          "name": "startAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=StartAssessmentRun?assessmentRunName=assessmentRunName&assessmentTemplateArn=assessmentTemplateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts the assessment run specified by the ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f818088c-6651-4ce2-ada5-f4cda44e44ed"
            }
          ]
        },
        {
          "id": "b541a2ee-88b1-4888-a7ee-95901b33300d",
          "name": "stopAssessmentRun",
          "request": {
            "url": "http://example.com/api/?Action=StopAssessmentRun?assessmentRunArn=assessmentRunArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stops the assessment run that is specified by the ARN of the assessment\n         run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7241750a-5ccd-4a5e-8182-08784c4e855e"
            }
          ]
        }
      ]
    },
    {
      "name": "Cross Account Access Roles",
      "item": [
        {
          "id": "056379fb-099c-4782-acd8-13196d484149",
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
              "id": "054d5e9d-919f-4f2c-8e84-cdb1bc15b3f9"
            }
          ]
        },
        {
          "id": "d5537541-d27d-4ba6-95b5-d6955797bd86",
          "name": "registerCrossAccountAccessRole",
          "request": {
            "url": "http://example.com/api/?Action=RegisterCrossAccountAccessRole?roleArn=roleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers the IAM role that Amazon Inspector uses to list your EC2 instances at the\n         start of the assessment run or when you call the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f17ff82d-a916-4d70-9d91-fd91d5d54e4d"
            }
          ]
        }
      ]
    },
    {
      "name": "Findings",
      "item": [
        {
          "id": "d9d28d7f-beca-4a02-a285-14568fbaa43d",
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
              "id": "ed73b4c5-a286-4e22-9e8e-8c5afc246dd9"
            }
          ]
        },
        {
          "id": "57f8719f-7031-4321-b9b5-da5ac84105a2",
          "name": "listFindings",
          "request": {
            "url": "http://example.com/api/?Action=ListFindings?assessmentRunArns=assessmentRunArns&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists findings that are generated by the assessment runs that are specified by the\n         ARNs of the assessment runs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee6c50d2-dfcc-4ede-bcf9-77a8402864de"
            }
          ]
        }
      ]
    },
    {
      "name": "Rules Packages",
      "item": [
        {
          "id": "23a3a491-202c-45ca-8ac3-523ca747e19c",
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
              "id": "6d16a0fa-f4cc-4ae6-99cc-934c47e4900f"
            }
          ]
        },
        {
          "id": "30dca7bb-397a-4496-b0b4-244e25026ae4",
          "name": "listRulesPackages",
          "request": {
            "url": "http://example.com/api/?Action=ListRulesPackages?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all available Amazon Inspector rules packages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "611dc963-451f-4899-913a-047e1fe5d5bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Telemetry Metadata",
      "item": [
        {
          "id": "6c16052e-184d-4c46-8196-568511d8fdce",
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
              "id": "8cdf9607-883e-4612-b2cc-8d5c7df043d3"
            }
          ]
        }
      ]
    },
    {
      "name": "Assessment Run Agents",
      "item": [
        {
          "id": "4d2201e4-20a9-4db5-b8c8-a2887993ca39",
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
              "id": "a9ecf3cd-9c33-4766-8cd7-abd50308c32b"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "93f02ae5-5e02-44ab-8f0b-bce4eb183abe",
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
              "id": "a97f2416-0da8-44f0-97a5-b3bbf6f62b7c"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags For Resources",
      "item": [
        {
          "id": "7e589dae-a7b7-4a07-ab80-7679febd8a90",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?resourceArn=resourceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags associated with an assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1afb77c-95ce-4d4d-b1d7-01a90e62c45a"
            }
          ]
        },
        {
          "id": "5d573699-8c0a-456d-b749-fe5dc6a469c2",
          "name": "setTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=SetTagsForResource?resourceArn=resourceArn&tags=tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets tags (key and value pairs) to the assessment template that is specified by the\n         ARN of the assessment template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6df0d7ab-87c5-4600-88a1-2ed863a1d912"
            }
          ]
        }
      ]
    },
    {
      "name": "Agents",
      "item": [
        {
          "id": "29f05fb3-efb8-4cf8-bdeb-6460073ee713",
          "name": "previewAgents",
          "request": {
            "url": "http://example.com/api/?Action=PreviewAgents?maxResults=maxResults&nextToken=nextToken&previewAgentsArn=previewAgentsArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Previews the agents installed on the EC2 instances that are part of the specified\n         assessment target."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c6470be-bd3d-4c6d-9f39-f41eaddac5c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Attributes From Findings",
      "item": [
        {
          "id": "90183c80-523b-485e-8ff3-442f66579f52",
          "name": "removeAttributesFromFindings",
          "request": {
            "url": "http://example.com/api/?Action=RemoveAttributesFromFindings?attributeKeys=attributeKeys&findingArns=findingArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes entire attributes (key and value pairs) from the findings that are specified\n         by the ARNs of the findings where an attribute with the specified key exists."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "574baf48-b767-47f0-a6d5-74bfa5b9832f"
            }
          ]
        }
      ]
    }
  ]
}