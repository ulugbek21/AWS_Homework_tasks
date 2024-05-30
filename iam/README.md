# AWS IAM Homework Tasks

## Task 1: Creating IAM Users and Groups

1. **Create IAM Users**:
   - Create three IAM users: `User1`, `User2`, and `User3`.
   - Provide each user with programmatic access by creating an access key.

2. **Create IAM Groups**:
   - Create two IAM groups: `AdminGroup` and `ReadOnlyGroup`.
   - Add `User1` to the `AdminGroup`.
   - Add `User2` and `User3` to the `ReadOnlyGroup`.

## Task 2: Assigning Policies to Groups

1. **Assign Policies**:
   - Attach the `AdministratorAccess` policy to the `AdminGroup`.
   - Attach the `ReadOnlyAccess` policy to the `ReadOnlyGroup`.

## Task 3: Creating Custom Policies

1. **Create a Custom Policy**:
   - Create a custom policy named `S3FullAccessPolicy` that allows full access to all S3 buckets.
   - Attach this policy to `User1`.

2. **Create a Policy Document**:
   - Write a JSON policy document that grants list and read permissions to a specific S3 bucket (`my-bucket`) and name it `S3ReadOnlyPolicy`.
   - Attach this policy to `User2`.

## Task 4: IAM Roles

1. **Create IAM Roles**:
   - Create a role named `EC2FullAccessRole` that grants full access to EC2 services.
   - Attach the `AmazonEC2FullAccess` policy to this role.

2. **Assign Role to EC2 Instance**:
   - Launch an EC2 instance and assign the `EC2FullAccessRole` to it.

## Task 5: MFA (Multi-Factor Authentication)

1. **Enable MFA**:
   - Enable MFA for `User1` using a virtual MFA device.
   - Document the steps taken to enable MFA and verify its configuration.

## Task 6: IAM Policy Simulator

1. **Policy Simulation**:
   - Use the IAM Policy Simulator to test the `S3ReadOnlyPolicy` attached to `User2`.
   - Verify that `User2` can list and read objects in the specified S3 bucket but cannot delete or upload objects.

## Task 7: Auditing IAM Activities

1. **View IAM Activity**:
   - Check the IAM user activity for `User1`, `User2`, and `User3` in CloudTrail.
   - Document any IAM-related activities performed by these users in the past day.

## Additional Instructions

- **Documentation**: Document each step taken in a report, including screenshots where applicable.
- **Submission**: Submit the report along with the policy JSON documents used in the tasks.
- **Review**: Be prepared to explain the reasoning behind each policy and role configuration in a follow-up discussion.
