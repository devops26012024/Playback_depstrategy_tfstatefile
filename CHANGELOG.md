
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

