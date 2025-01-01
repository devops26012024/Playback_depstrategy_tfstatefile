
## Version 1

### Changes:

Terraform will perform the following actions:

[1m  # aws_instance.ec2[0m will be updated in-place
[0m  [33m~[0m[0m resource "aws_instance" "ec2" {
        id                                   = "i-09438da35b09db89f"
      [33m~[0m[0m tags                                 = {
          [33m~[0m[0m "Name"    = "Feb2nd" [33m->[0m[0m "Jan1st"
            "Version" = "v1.0.0"
        }
      [33m~[0m[0m tags_all                             = {
          [33m~[0m[0m "Name"    = "Feb2nd" [33m->[0m[0m "Jan1st"
            [90m# (1 unchanged element hidden)[0m[0m
        }
        [90m# (30 unchanged attributes hidden)[0m[0m

        [90m# (8 unchanged blocks hidden)[0m[0m
    }

[0m::debug::Terraform exited with code 0.
::debug::stderr: 
::debug::exitcode: 0

## Version 2

### Changes:

Terraform will perform the following actions:

[1m  # aws_instance.ec2[0m will be created
[0m  [32m+[0m[0m resource "aws_instance" "ec2" {
      [32m+[0m[0m ami                                  = "ami-053b12d3152c0cc71"
      [32m+[0m[0m arn                                  = (known after apply)
      [32m+[0m[0m associate_public_ip_address          = (known after apply)
      [32m+[0m[0m availability_zone                    = (known after apply)
      [32m+[0m[0m cpu_core_count                       = (known after apply)
      [32m+[0m[0m cpu_threads_per_core                 = (known after apply)
      [32m+[0m[0m disable_api_stop                     = (known after apply)
      [32m+[0m[0m disable_api_termination              = (known after apply)
      [32m+[0m[0m ebs_optimized                        = (known after apply)
      [32m+[0m[0m enable_primary_ipv6                  = (known after apply)
      [32m+[0m[0m get_password_data                    = false
      [32m+[0m[0m host_id                              = (known after apply)
      [32m+[0m[0m host_resource_group_arn              = (known after apply)
      [32m+[0m[0m iam_instance_profile                 = (known after apply)
      [32m+[0m[0m id                                   = (known after apply)
      [32m+[0m[0m instance_initiated_shutdown_behavior = (known after apply)
      [32m+[0m[0m instance_lifecycle                   = (known after apply)
      [32m+[0m[0m instance_state                       = (known after apply)
      [32m+[0m[0m instance_type                        = "t2.micro"
      [32m+[0m[0m ipv6_address_count                   = (known after apply)
      [32m+[0m[0m ipv6_addresses                       = (known after apply)
      [32m+[0m[0m key_name                             = (known after apply)
      [32m+[0m[0m monitoring                           = (known after apply)
      [32m+[0m[0m outpost_arn                          = (known after apply)
      [32m+[0m[0m password_data                        = (known after apply)
      [32m+[0m[0m placement_group                      = (known after apply)
      [32m+[0m[0m placement_partition_number           = (known after apply)
      [32m+[0m[0m primary_network_interface_id         = (known after apply)
      [32m+[0m[0m private_dns                          = (known after apply)
      [32m+[0m[0m private_ip                           = (known after apply)
      [32m+[0m[0m public_dns                           = (known after apply)
      [32m+[0m[0m public_ip                            = (known after apply)
      [32m+[0m[0m secondary_private_ips                = (known after apply)
      [32m+[0m[0m security_groups                      = [
          [32m+[0m[0m "ec2-security-group",
        ]
      [32m+[0m[0m source_dest_check                    = true
      [32m+[0m[0m spot_instance_request_id             = (known after apply)
      [32m+[0m[0m subnet_id                            = (known after apply)
      [32m+[0m[0m tags                                 = {
          [32m+[0m[0m "Name"    = "Jan1st"
          [32m+[0m[0m "Version" = "v1.0.0"
        }
      [32m+[0m[0m tags_all                             = {
          [32m+[0m[0m "Name"    = "Jan1st"
          [32m+[0m[0m "Version" = "v1.0.0"
        }
      [32m+[0m[0m tenancy                              = (known after apply)
      [32m+[0m[0m user_data                            = (known after apply)
      [32m+[0m[0m user_data_base64                     = (known after apply)
      [32m+[0m[0m user_data_replace_on_change          = false
      [32m+[0m[0m vpc_security_group_ids               = (known after apply)
    }

[1m  # aws_security_group.ec2_sg[0m will be created
[0m  [32m+[0m[0m resource "aws_security_group" "ec2_sg" {
      [32m+[0m[0m arn                    = (known after apply)
      [32m+[0m[0m description            = "Allow SSH traffic"
      [32m+[0m[0m egress                 = [
          [32m+[0m[0m {
              [32m+[0m[0m cidr_blocks      = [
                  [32m+[0m[0m "0.0.0.0/0",
                ]
              [32m+[0m[0m description      = ""
              [32m+[0m[0m from_port        = 0
              [32m+[0m[0m ipv6_cidr_blocks = []
              [32m+[0m[0m prefix_list_ids  = []
              [32m+[0m[0m protocol         = "-1"
              [32m+[0m[0m security_groups  = []
              [32m+[0m[0m self             = false
              [32m+[0m[0m to_port          = 0
            },
        ]
      [32m+[0m[0m id                     = (known after apply)
      [32m+[0m[0m ingress                = [
          [32m+[0m[0m {
              [32m+[0m[0m cidr_blocks      = [
                  [32m+[0m[0m "0.0.0.0/0",
                ]
              [32m+[0m[0m description      = ""
              [32m+[0m[0m from_port        = 22
              [32m+[0m[0m ipv6_cidr_blocks = []
              [32m+[0m[0m prefix_list_ids  = []
              [32m+[0m[0m protocol         = "tcp"
              [32m+[0m[0m security_groups  = []
              [32m+[0m[0m self             = false
              [32m+[0m[0m to_port          = 22
            },
        ]
      [32m+[0m[0m name                   = "ec2-security-group"
      [32m+[0m[0m name_prefix            = (known after apply)
      [32m+[0m[0m owner_id               = (known after apply)
      [32m+[0m[0m revoke_rules_on_delete = false
      [32m+[0m[0m tags                   = {
          [32m+[0m[0m "Name" = "EC2SecurityGroup"
        }
      [32m+[0m[0m tags_all               = {
--
::debug::stderr: 
::debug::exitcode: 0

