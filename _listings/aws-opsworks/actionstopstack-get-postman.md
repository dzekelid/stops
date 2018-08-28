{
  "info": {
    "name": "AWS OpsWorks API Stop Stack",
    "_postman_id": "4bb6daf0-d45f-4096-9712-56c03e010903",
    "description": "Stops a specified stack.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instances",
      "item": [
        {
          "id": "1679fef1-7cb4-48c3-aaa1-2566de74b9f1",
          "name": "assignInstance",
          "request": {
            "url": "http://example.com/api/?Action=AssignInstance?InstanceId=InstanceId&LayerIds=LayerIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assign a registered instance to a layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78478558-b246-4270-a658-1291707c7a16"
            }
          ]
        },
        {
          "id": "0901e599-adfb-4cdd-b086-20ced5641fba",
          "name": "createInstance",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstance?AgentVersion=AgentVersion&AmiId=AmiId&Architecture=Architecture&AutoScalingType=AutoScalingType&AvailabilityZone=AvailabilityZone&BlockDeviceMappings=BlockDeviceMappings&EbsOptimized=EbsOptimized&Hostname=Hostname&InstallUpdatesOnBoot=InstallUpdatesOnBoot&InstanceType=InstanceType&LayerIds=LayerIds&Os=Os&RootDeviceType=RootDeviceType&SshKeyName=SshKeyName&StackId=StackId&SubnetId=SubnetId&Tenancy=Tenancy&VirtualizationType=VirtualizationType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an instance in a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80f8ed7c-1c2d-4c94-879d-95d351d31016"
            }
          ]
        },
        {
          "id": "81544e90-a054-43f5-80be-06158209213e",
          "name": "deleteInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteInstance?DeleteElasticIp=DeleteElasticIp&DeleteVolumes=DeleteVolumes&InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified instance, which terminates the associated Amazon EC2 instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad35cb91-19d4-4313-9e63-3c24f37f67e6"
            }
          ]
        },
        {
          "id": "675976ee-f89d-44ee-9d25-073ee79d67ce",
          "name": "deregisterInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregister a registered Amazon EC2 or on-premises instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b124a502-930d-4d97-8178-6aa5f27a0092"
            }
          ]
        },
        {
          "id": "64a00fc0-6e48-4024-8e9c-d65b34ae57fb",
          "name": "deregisterRdsDbInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterRdsDbInstance?RdsDbInstanceArn=RdsDbInstanceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters an Amazon RDS instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a314ee56-9334-48da-8db2-22f644ab8192"
            }
          ]
        },
        {
          "id": "761c9758-28cc-41e6-b9a8-60dfdf147351",
          "name": "describeInstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstances?InstanceIds=InstanceIds&LayerId=LayerId&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of a set of instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9ebd02a-86dd-4029-b49f-949b9d0dfba9"
            }
          ]
        },
        {
          "id": "07d00b4e-826d-4090-8da2-0b4566b3d61e",
          "name": "describeRdsDbInstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRdsDbInstances?RdsDbInstanceArns=RdsDbInstanceArns&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes Amazon RDS instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "505efd2c-beb2-4841-9f6b-e483413b3c9d"
            }
          ]
        },
        {
          "id": "13096f51-c933-446b-8f0c-17c741d6804a",
          "name": "rebootInstance",
          "request": {
            "url": "http://example.com/api/?Action=RebootInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Reboots a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73ab50a2-3c61-4e46-b83e-744de020b4ef"
            }
          ]
        },
        {
          "id": "45cdde38-eb00-44c8-9fe4-4db308d357e9",
          "name": "registerInstance",
          "request": {
            "url": "http://example.com/api/?Action=RegisterInstance?Hostname=Hostname&InstanceIdentity=InstanceIdentity&PrivateIp=PrivateIp&PublicIp=PublicIp&RsaPublicKey=RsaPublicKey&RsaPublicKeyFingerprint=RsaPublicKeyFingerprint&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers instances that were created outside of AWS OpsWorks Stacks with a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0faa7368-cd77-48c7-aba2-ff68202409ec"
            }
          ]
        },
        {
          "id": "180a448e-44ff-4ad0-b182-f68c1643ef16",
          "name": "registerRdsDbInstance",
          "request": {
            "url": "http://example.com/api/?Action=RegisterRdsDbInstance?DbPassword=DbPassword&DbUser=DbUser&RdsDbInstanceArn=RdsDbInstanceArn&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers an Amazon RDS instance with a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0df79ec-0c89-41fd-8479-b5428483ccd7"
            }
          ]
        },
        {
          "id": "9a94989b-b10f-4fff-bbf1-7b8da505269e",
          "name": "startInstance",
          "request": {
            "url": "http://example.com/api/?Action=StartInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c55cfb72-ad35-4612-a1bb-3e26acc219a7"
            }
          ]
        },
        {
          "id": "76522441-4de7-47c1-aa91-cef8ff50e5eb",
          "name": "stopInstance",
          "request": {
            "url": "http://example.com/api/?Action=StopInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stops a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34b79312-75f4-4221-a609-e5d990d49463"
            }
          ]
        }
      ]
    },
    {
      "name": "Volumes",
      "item": [
        {
          "id": "37d2690f-3ad1-45cc-8d68-8143b8b0a6bd",
          "name": "assignVolume",
          "request": {
            "url": "http://example.com/api/?Action=AssignVolume?InstanceId=InstanceId&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Assigns one of the stack's registered Amazon EBS volumes to a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a1826f8-27b5-443b-bbf2-6b9e9aa236ad"
            }
          ]
        },
        {
          "id": "4d186be2-e5fb-4b32-bb16-bdafaf7a7a24",
          "name": "deregisterVolume",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterVolume?VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters an Amazon EBS volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfb91bbe-7d5f-44fd-97a2-289f4f04c0b2"
            }
          ]
        },
        {
          "id": "569fdb1b-00a4-4273-a796-cb174335a512",
          "name": "describeVolumes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeVolumes?InstanceId=InstanceId&RaidArrayId=RaidArrayId&StackId=StackId&VolumeIds=VolumeIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes an instance's Amazon EBS volumes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ccfd801-8507-4207-a3d3-2cfe1c42d7bc"
            }
          ]
        },
        {
          "id": "e04984d4-3b80-45d9-8b09-048c9e2ed5a2",
          "name": "registerVolume",
          "request": {
            "url": "http://example.com/api/?Action=RegisterVolume?Ec2VolumeId=Ec2VolumeId&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers an Amazon EBS volume with a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04516f2c-8e9e-4c97-8d67-5d38feed12cd"
            }
          ]
        }
      ]
    },
    {
      "name": "IP Addresses",
      "item": [
        {
          "id": "7c76a9f7-0fa1-4ed8-8b9d-cb6680ef864d",
          "name": "associateElasticIp",
          "request": {
            "url": "http://example.com/api/?Action=AssociateElasticIp?ElasticIp=ElasticIp&InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates one of the stack's registered Elastic IP addresses with a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61a3d265-632a-41e1-8492-7c2a228380f2"
            }
          ]
        },
        {
          "id": "7d3aea14-e97a-4adb-8215-8dcb10898fbe",
          "name": "deregisterElasticIp",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterElasticIp?ElasticIp=ElasticIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters a specified Elastic IP address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "080ad1de-7978-498f-ba44-1920bbd5c004"
            }
          ]
        },
        {
          "id": "a6aa130a-51e6-4288-9467-0a4d488c9b36",
          "name": "describeElasticIps",
          "request": {
            "url": "http://example.com/api/?Action=DescribeElasticIps?InstanceId=InstanceId&Ips=Ips&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes Elastic IPs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d082233-2e2d-4569-bb22-7d8ee7ed2520"
            }
          ]
        },
        {
          "id": "71d3c5aa-4508-4757-ab9e-e6fb2d5be27b",
          "name": "disassociateElasticIp",
          "request": {
            "url": "http://example.com/api/?Action=DisassociateElasticIp?ElasticIp=ElasticIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates an Elastic IP address from its instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd20a906-b541-493b-8706-fbff47aeff10"
            }
          ]
        },
        {
          "id": "13de6ba4-13d7-4e31-a367-47444c6595ad",
          "name": "registerElasticIp",
          "request": {
            "url": "http://example.com/api/?Action=RegisterElasticIp?ElasticIp=ElasticIp&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers an Elastic IP address with a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d977a8f-b697-4e25-b1f9-fef753a94577"
            }
          ]
        }
      ]
    },
    {
      "name": "Load Balancers",
      "item": [
        {
          "id": "61509f98-6cd4-472d-bd80-05a41d6eb800",
          "name": "attachElasticLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=AttachElasticLoadBalancer?ElasticLoadBalancerName=ElasticLoadBalancerName&LayerId=LayerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches an Elastic Load Balancing load balancer to a specified layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac4c6c08-f150-49e9-8c81-2bfc07458bf9"
            }
          ]
        },
        {
          "id": "5123f23c-5cc9-46d9-b8e3-ebb4e97e4983",
          "name": "describeElasticLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DescribeElasticLoadBalancers?LayerIds=LayerIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a stack's Elastic Load Balancing instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34148852-3974-42d0-8e33-4fa6dd3dd035"
            }
          ]
        },
        {
          "id": "c143c132-8462-4910-b491-94e3295e656d",
          "name": "detachElasticLoadBalancer",
          "request": {
            "url": "http://example.com/api/?Action=DetachElasticLoadBalancer?ElasticLoadBalancerName=ElasticLoadBalancerName&LayerId=LayerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches a specified Elastic Load Balancing instance from its layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fd428db-4cb3-45b3-92fb-1f77f11bdd21"
            }
          ]
        }
      ]
    },
    {
      "name": "Stacks",
      "item": [
        {
          "id": "0064c8f8-569a-49bb-8b5d-990eed1f6320",
          "name": "cloneStack",
          "request": {
            "url": "http://example.com/api/?Action=CloneStack?AgentVersion=AgentVersion&Attributes=Attributes&ChefConfiguration=ChefConfiguration&CloneAppIds=CloneAppIds&ClonePermissions=ClonePermissions&ConfigurationManager=ConfigurationManager&CustomCookbooksSource=CustomCookbooksSource&CustomJson=CustomJson&DefaultAvailabilityZone=DefaultAvailabilityZone&DefaultInstanceProfileArn=DefaultInstanceProfileArn&DefaultOs=DefaultOs&DefaultRootDeviceType=DefaultRootDeviceType&DefaultSshKeyName=DefaultSshKeyName&DefaultSubnetId=DefaultSubnetId&HostnameTheme=HostnameTheme&Name=Name&Region=Region&ServiceRoleArn=ServiceRoleArn&SourceStackId=SourceStackId&UseCustomCookbooks=UseCustomCookbooks&UseOpsworksSecurityGroups=UseOpsworksSecurityGroups&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a clone of a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50b7d999-0ba7-4d11-8d89-f6d44a580494"
            }
          ]
        },
        {
          "id": "d1c616d7-fa0d-4d2f-bae5-29c1ecbe9470",
          "name": "describeStackProvisioningParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackProvisioningParameters?StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of a stack's provisioning parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1716c62c-3450-4cd5-a739-703cd7753a2e"
            }
          ]
        },
        {
          "id": "bd680915-73cf-4d86-98ae-cd28fd9bef45",
          "name": "describeStacks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStacks?StackIds=StackIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of one or more stacks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58fb8f79-434a-4e0f-88a1-2574318b13d9"
            }
          ]
        },
        {
          "id": "6da6a489-6134-4ba3-b046-33f072b5f1ae",
          "name": "describeStackSummary",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackSummary?StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the number of layers and apps in a specified stack, and the number of instances in\n      each state, such as running_setup or online."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8fa53c53-61f3-4161-bc1f-3412258dc32a"
            }
          ]
        },
        {
          "id": "37ac4c83-97f2-4217-8e42-e662871e300c",
          "name": "startStack",
          "request": {
            "url": "http://example.com/api/?Action=StartStack?StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts a stack's instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8a28f0a-58b2-453c-a27e-7a605720cf3d"
            }
          ]
        },
        {
          "id": "381033de-40c6-4785-96ff-9ba4d850b574",
          "name": "stopStack",
          "request": {
            "url": "http://example.com/api/?Action=StopStack?StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stops a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3e622f3-33a6-4005-9f41-c13e489895b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Applications",
      "item": [
        {
          "id": "46cfdcb5-ad4d-4be6-b458-84400b4aff22",
          "name": "createApp",
          "request": {
            "url": "http://example.com/api/?Action=CreateApp?AppSource=AppSource&Attributes=Attributes&DataSources=DataSources&Description=Description&Domains=Domains&EnableSsl=EnableSsl&Environment=Environment&Name=Name&Shortname=Shortname&SslConfiguration=SslConfiguration&StackId=StackId&Type=Type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an app for a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "475eeed4-ed13-4710-9712-a934d6d3812e"
            }
          ]
        },
        {
          "id": "202a270f-ed21-4e32-81f2-c17da2852660",
          "name": "deleteApp",
          "request": {
            "url": "http://example.com/api/?Action=DeleteApp?AppId=AppId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28f35e38-3bae-4823-bbb8-55c552a9859b"
            }
          ]
        },
        {
          "id": "6c99c115-ce77-4811-83c2-2a5f246f31b2",
          "name": "describeApps",
          "request": {
            "url": "http://example.com/api/?Action=DescribeApps?AppIds=AppIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of a specified set of apps."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5743161-4019-4453-8cc4-93f55d53995a"
            }
          ]
        }
      ]
    },
    {
      "name": "Folder",
      "item": [
        {
          "id": "96f41f5e-b6c1-43bb-a5db-901f67dbe9af",
          "name": "createDeployment",
          "request": {
            "url": "http://example.com/api/?Action=CreateDeployment?AppId=AppId&Command=Command&Comment=Comment&CustomJson=CustomJson&InstanceIds=InstanceIds&LayerIds=LayerIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Runs deployment or stack commands."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "327074a5-915f-43e1-a794-4d8f8d71fdac"
            }
          ]
        },
        {
          "id": "263007be-2871-45c7-9e5f-a06f42c90eef",
          "name": "createLayer",
          "request": {
            "url": "http://example.com/api/?Action=CreateLayer?Attributes=Attributes&AutoAssignElasticIps=AutoAssignElasticIps&AutoAssignPublicIps=AutoAssignPublicIps&CustomInstanceProfileArn=CustomInstanceProfileArn&CustomJson=CustomJson&CustomRecipes=CustomRecipes&CustomSecurityGroupIds=CustomSecurityGroupIds&EnableAutoHealing=EnableAutoHealing&InstallUpdatesOnBoot=InstallUpdatesOnBoot&LifecycleEventConfiguration=LifecycleEventConfiguration&Name=Name&Packages=Packages&Shortname=Shortname&StackId=StackId&Type=Type&UseEbsOptimizedInstances=UseEbsOptimizedInstances&VolumeConfigurations=VolumeConfigurations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62ca30e7-345e-43b1-8d8e-43c47004870a"
            }
          ]
        },
        {
          "id": "55936fd6-f5df-4de1-8ad5-5ac601e43dc5",
          "name": "createStack",
          "request": {
            "url": "http://example.com/api/?Action=CreateStack?AgentVersion=AgentVersion&Attributes=Attributes&ChefConfiguration=ChefConfiguration&ConfigurationManager=ConfigurationManager&CustomCookbooksSource=CustomCookbooksSource&CustomJson=CustomJson&DefaultAvailabilityZone=DefaultAvailabilityZone&DefaultInstanceProfileArn=DefaultInstanceProfileArn&DefaultOs=DefaultOs&DefaultRootDeviceType=DefaultRootDeviceType&DefaultSshKeyName=DefaultSshKeyName&DefaultSubnetId=DefaultSubnetId&HostnameTheme=HostnameTheme&Name=Name&Region=Region&ServiceRoleArn=ServiceRoleArn&UseCustomCookbooks=UseCustomCookbooks&UseOpsworksSecurityGroups=UseOpsworksSecurityGroups&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60973ef4-4b15-4531-9f8d-9cffc3340c02"
            }
          ]
        },
        {
          "id": "3466bde3-3c9a-463c-a436-241b7acf679f",
          "name": "createUserProfile",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserProfile?AllowSelfManagement=AllowSelfManagement&IamUserArn=IamUserArn&SshPublicKey=SshPublicKey&SshUsername=SshUsername",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new user profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01302593-902b-45f6-bfab-e5147ae98b09"
            }
          ]
        },
        {
          "id": "cd6539eb-93cb-45e7-a8c4-994566d99ef8",
          "name": "deleteLayer",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLayer?LayerId=LayerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b822076-97f2-4aec-a079-0fd014b16fbd"
            }
          ]
        },
        {
          "id": "d3eb2741-6d89-4f63-ae30-194e7cb41854",
          "name": "deleteStack",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStack?StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85feea9f-13cf-4ea0-b355-3cdef645b403"
            }
          ]
        },
        {
          "id": "d6a7833f-66a2-4dc2-918f-5bf6a91e599a",
          "name": "deleteUserProfile",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserProfile?IamUserArn=IamUserArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a user profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43e0149e-a24d-41a5-b2af-9a795fff3c9f"
            }
          ]
        },
        {
          "id": "4faaa9dc-7cc7-4def-81e6-a39287698fe0",
          "name": "deregisterEcsCluster",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterEcsCluster?EcsClusterArn=EcsClusterArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters a specified Amazon ECS cluster from a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d869bd88-b646-485c-9df0-3670c2be96ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Agent Versions",
      "item": [
        {
          "id": "76712b5c-290d-4615-9d1f-e0b74aec6d05",
          "name": "describeAgentVersions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAgentVersions?ConfigurationManager=ConfigurationManager&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available AWS OpsWorks Stacks agent versions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f78e9f44-b7a2-459a-b2a6-0ebc5a2a04fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Commands",
      "item": [
        {
          "id": "d5ebae3b-1eb2-4bc0-b84c-b067ff65658b",
          "name": "describeCommands",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCommands?CommandIds=CommandIds&DeploymentId=DeploymentId&InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the results of specified commands."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a3c1902-aa5a-4c95-bfc5-219e17691e11"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployments",
      "item": [
        {
          "id": "67d62c6a-7434-4866-abee-b29c8c7fd87d",
          "name": "describeDeployments",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDeployments?AppId=AppId&DeploymentIds=DeploymentIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of a specified set of deployments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73e3a3d6-7dfa-468d-94a1-4bfadaa24860"
            }
          ]
        }
      ]
    },
    {
      "name": "ECS Clusters",
      "item": [
        {
          "id": "9c4875d5-ebf5-4f34-b940-86c88d6dbb46",
          "name": "describeEcsClusters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEcsClusters?EcsClusterArns=EcsClusterArns&MaxResults=MaxResults&NextToken=NextToken&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes Amazon ECS clusters that are registered with a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "927ac30e-f080-41ac-aadb-6e3df7b84a03"
            }
          ]
        },
        {
          "id": "28a75eb7-6248-49b5-8bd9-b58425da4b59",
          "name": "registerEcsCluster",
          "request": {
            "url": "http://example.com/api/?Action=RegisterEcsCluster?EcsClusterArn=EcsClusterArn&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a specified Amazon ECS cluster with a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47865583-cb05-4afe-8db3-04e37c86f658"
            }
          ]
        }
      ]
    },
    {
      "name": "Layers",
      "item": [
        {
          "id": "296d919f-48ef-464d-a2af-4587e1caef86",
          "name": "describeLayers",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLayers?LayerIds=LayerIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests a description of one or more layers in a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c61aa7b-eb22-4b76-873f-b48bd199c39c"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling",
      "item": [
        {
          "id": "0b12b4cf-3bc4-4194-bc00-bcabf3083160",
          "name": "describeLoadBasedAutoScaling",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBasedAutoScaling?LayerIds=LayerIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes load-based auto scaling configurations for specified layers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "124ad8c7-2221-4179-9076-7bfd0ad3f030"
            }
          ]
        },
        {
          "id": "541f60f6-797d-4677-abd3-d4188f6bfb9b",
          "name": "describeTimeBasedAutoScaling",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTimeBasedAutoScaling?InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes time-based auto scaling configurations for specified instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c9fdd0e-4c7c-4a43-9ebf-2c8afa44edd7"
            }
          ]
        },
        {
          "id": "66697af5-5400-4df9-9cb0-27e686dff008",
          "name": "setLoadBasedAutoScaling",
          "request": {
            "url": "http://example.com/api/?Action=SetLoadBasedAutoScaling?DownScaling=DownScaling&Enable=Enable&LayerId=LayerId&UpScaling=UpScaling",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specify the load-based auto scaling configuration for a specified layer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef5a8a8a-8207-4231-9316-481d375b40b8"
            }
          ]
        },
        {
          "id": "c4986b74-eeaa-4af3-bdc0-0973517d5fa8",
          "name": "setTimeBasedAutoScaling",
          "request": {
            "url": "http://example.com/api/?Action=SetTimeBasedAutoScaling?AutoScalingSchedule=AutoScalingSchedule&InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specify the time-based auto scaling configuration for a specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24687cf9-879e-4a50-99b2-045a2fb967ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "92246830-3937-4ee4-af6e-f51264221793",
          "name": "describeMyUserProfile",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMyUserProfile?UserProfile=UserProfile",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a user's SSH information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c52cd6c7-6738-430f-9738-cd31e2a93cd9"
            }
          ]
        },
        {
          "id": "7d6b9e73-3177-443f-9614-381ddec1d507",
          "name": "describeUserProfiles",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserProfiles?IamUserArns=IamUserArns",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describe specified users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7809de93-6bfd-471f-abcf-e44f975c6793"
            }
          ]
        }
      ]
    },
    {
      "name": "Permissions",
      "item": [
        {
          "id": "5bae25b3-59fb-4c5e-bcde-a9e5221adac5",
          "name": "describePermissions",
          "request": {
            "url": "http://example.com/api/?Action=DescribePermissions?IamUserArn=IamUserArn&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the permissions for a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4de75a7-1d56-4ba3-87f0-e85bbc4149e8"
            }
          ]
        },
        {
          "id": "43af4a81-98c7-413a-91fe-d2ea415dd20d",
          "name": "setPermission",
          "request": {
            "url": "http://example.com/api/?Action=SetPermission?AllowSsh=AllowSsh&AllowSudo=AllowSudo&IamUserArn=IamUserArn&Level=Level&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specifies a user's permissions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5eb6e98f-e1da-4dd8-bd39-b24bcc173d05"
            }
          ]
        }
      ]
    },
    {
      "name": "Raid Arrays",
      "item": [
        {
          "id": "a5fbcbde-9293-4a4c-b524-5915e8e671ee",
          "name": "describeRaidArrays",
          "request": {
            "url": "http://example.com/api/?Action=DescribeRaidArrays?InstanceId=InstanceId&RaidArrayIds=RaidArrayIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describe an instance's RAID arrays."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40a3bca2-52d5-460b-a550-49142b2b4093"
            }
          ]
        }
      ]
    },
    {
      "name": "Service Errors",
      "item": [
        {
          "id": "0943d4a9-d20c-4eb9-9c78-8308c8ae9077",
          "name": "describeServiceErrors",
          "request": {
            "url": "http://example.com/api/?Action=DescribeServiceErrors?InstanceId=InstanceId&ServiceErrorIds=ServiceErrorIds&StackId=StackId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes AWS OpsWorks Stacks service errors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16442427-3851-4ac1-9bb8-6afee66690f3"
            }
          ]
        }
      ]
    },
    {
      "name": "Host Names",
      "item": [
        {
          "id": "28f5feb0-ea6c-423e-933a-8489c283aebe",
          "name": "getHostnameSuggestion",
          "request": {
            "url": "http://example.com/api/?Action=GetHostnameSuggestion?LayerId=LayerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a generated host name for the specified layer, based on the current host name theme."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6159d5d8-a2b6-4ef6-aa13-fc7a8fb69dbf"
            }
          ]
        }
      ]
    },
    {
      "name": "Access",
      "item": [
        {
          "id": "6ecb1388-94ab-4713-ae92-a76b11f90827",
          "name": "grantAccess",
          "request": {
            "url": "http://example.com/api/?Action=GrantAccess?InstanceId=InstanceId&ValidForInMinutes=ValidForInMinutes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "NoteThis action can be used only with Windows stacks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2312c2e6-f82d-45a4-ab33-c93e832f9a92"
            }
          ]
        }
      ]
    }
  ]
}