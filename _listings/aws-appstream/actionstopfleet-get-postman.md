{
  "info": {
    "name": "AWS AppStream 2.0 API Stop Fleet",
    "_postman_id": "4c73d390-d5f0-4757-b5ea-96f9a2668077",
    "description": "Stops a fleet.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fleet",
      "item": [
        {
          "id": "e6dd514a-9605-45c5-9f5c-254ea2e50859",
          "name": "AssociateFleet",
          "request": {
            "url": "http://example.com/api/?Action=AssociateFleet?FleetName=FleetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associate a fleet to a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52f8e721-8332-48b1-b635-8b0d734c2a1f"
            }
          ]
        },
        {
          "id": "cd25f057-b25a-4ab3-826a-dfccedf9df8c",
          "name": "CreateFleet",
          "request": {
            "url": "http://example.com/api/?Action=CreateFleet?ComputeCapacity=ComputeCapacity&Description=Description&DisconnectTimeoutInSeconds=DisconnectTimeoutInSeconds&DisplayName=DisplayName&ImageName=ImageName&InstanceType=InstanceType&MaxUserDurationInSeconds=MaxUserDurationInSeconds&Name=Name&VpcConfig=VpcConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84869b95-f286-4468-88ab-6305bc1260c0"
            }
          ]
        },
        {
          "id": "5779973f-0b2a-4e7c-81d5-199729790e89",
          "name": "CreateStack",
          "request": {
            "url": "http://example.com/api/?Action=CreateStack?Description=Description&DisplayName=DisplayName&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01c283dc-9469-4c64-b9b0-99a5d4aa6ded"
            }
          ]
        },
        {
          "id": "6abe68c2-3f53-43a1-bc89-4cef5bbf1a3b",
          "name": "DeleteFleet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteFleet?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfd27539-7b23-43b7-8c1a-626f6e13fc3d"
            }
          ]
        },
        {
          "id": "84960ee4-2a1e-428d-a060-ff52be05641b",
          "name": "DescribeFleets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeFleets?Names=Names&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If fleet names are provided, this operation describes the specified fleets;\n            otherwise, all the fleets in the account are described."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1213e116-6dba-4867-b592-6f796b1fdbdf"
            }
          ]
        },
        {
          "id": "211a702b-3eca-42de-984b-2ad2d50ac27a",
          "name": "DisassociateFleet",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateFleet?FleetName=FleetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates a fleet from a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2912239-1c61-4d52-83c4-744cc1ed688b"
            }
          ]
        },
        {
          "id": "85bc3772-4773-4b6e-94fe-ae86b0fe8fad",
          "name": "ListAssociatedFleets",
          "request": {
            "url": "http://example.com/api/?Action=ListAssociatedFleets?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all fleets associated with the stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4923e19d-ec08-4587-a7cb-cd12bd5ef69d"
            }
          ]
        },
        {
          "id": "3d9e76b1-3869-4419-98c1-30583790dfd7",
          "name": "StartFleet",
          "request": {
            "url": "http://example.com/api/?Action=StartFleet?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5e89ac9-0ace-4b67-b6d4-313a98b20db3"
            }
          ]
        },
        {
          "id": "c1b4a070-894b-4aad-80f6-f88286abbf45",
          "name": "StopFleet",
          "request": {
            "url": "http://example.com/api/?Action=StopFleet?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stops a fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55513065-e3c4-44eb-ac14-779863efae47"
            }
          ]
        }
      ]
    },
    {
      "name": "URL",
      "item": [
        {
          "id": "4f203bac-5003-4601-b61e-5e6264ae130f",
          "name": "CreateStreamingURL",
          "request": {
            "url": "http://example.com/api/?Action=CreateStreamingURL?ApplicationId=ApplicationId&FleetName=FleetName&SessionContext=SessionContext&StackName=StackName&UserId=UserId&Validity=Validity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a URL to start an AppStream 2."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5bbe1e2-c079-40e3-94ae-3d8468bbd695"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack",
      "item": [
        {
          "id": "3d0075be-4053-4aa8-a8eb-8bfafdb82ece",
          "name": "DeleteStack",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStack?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca6c5c79-6e7d-4bed-9382-e9ad9af77820"
            }
          ]
        },
        {
          "id": "54adf7d8-f690-4b0e-9fe9-5244f746750c",
          "name": "ListAssociatedStacks",
          "request": {
            "url": "http://example.com/api/?Action=ListAssociatedStacks?FleetName=FleetName&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all stacks to which the specified fleet is associated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15260c4b-7872-4ef6-8015-6fa99f362a04"
            }
          ]
        }
      ]
    },
    {
      "name": "Images",
      "item": [
        {
          "id": "fac69410-92d3-4ea5-a90b-32801c9b10e1",
          "name": "DescribeImages",
          "request": {
            "url": "http://example.com/api/?Action=DescribeImages?Names=Names",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b73fef1-24dc-434f-b87c-ee9e0bfbdd7f"
            }
          ]
        }
      ]
    },
    {
      "name": "Sessions",
      "item": [
        {
          "id": "f871b64a-8ddd-4bbb-b7f6-8278d76c93d3",
          "name": "DescribeSessions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSessions?FleetName=FleetName&Limit=Limit&NextToken=NextToken&StackName=StackName&UserId=UserId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the streaming sessions for a stack and a fleet."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94d15034-a79d-44fd-a3bb-6ac4cda7b9ce"
            }
          ]
        }
      ]
    },
    {
      "name": "Stacks",
      "item": [
        {
          "id": "d255df09-040d-45b2-bfca-801f641860ef",
          "name": "DescribeStacks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStacks?Names=Names&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If stack names are not provided, this operation describes the specified stacks;\n            otherwise, all stacks in the account are described."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "260a08ce-8453-4c67-81fa-233bb2b24b23"
            }
          ]
        }
      ]
    },
    {
      "name": "Session",
      "item": [
        {
          "id": "db60e9e7-21d4-4f08-a4fa-a6df36b430ff",
          "name": "ExpireSession",
          "request": {
            "url": "http://example.com/api/?Action=ExpireSession?SessionId=SessionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This operation immediately stops a streaming session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31ad71e2-456b-4a42-be8c-544a7533c463"
            }
          ]
        }
      ]
    }
  ]
}