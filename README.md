<!-- Start with a short description that explains what the offering is, why a customer would want to
install and use it, etc. The following info is used here as an example. Be sure to update it
accordingly. -->

Do you want to move?  Let us doing the heavy lifting and movey our busy workloads.  Just lean back
and kick up your legs and we will do all the work for you.

***Let's go!***

## Before you begin

<!-- List any prereqs including required permissions, capacity requirements, etc. The following info
is used as an example. Update accordingly. -->

* N/A

## Required resources

<!-- The following info is used here as an example. Be sure to update it accordingly. -->

To run the software, the following resources are required:

  * IBM VPC Account 

## Costs
Do you really think this is free?  Of course, it will be free as a trial offering.

## Installing the software

<!-- Recommendation is to not include the large table of configuration parameters that are listed on
the Create page. -->

### Production configuration

<!-- Add additional H3 level headings as needed for sections that apply to use on IBM Cloud such as
network policy, persistence, cluster topologies, etc.
### H3
### H3
-->

## Upgrading to a new version

<!-- How can a user upgrade to a new version when it's available? The following info is used as an
example. Update accordingly. -->

When a new version of a Rackware RMM is available, you're alerted in your Schematics workspace. To
upgrade to a new version, complete the following steps:

1. Go to the **Menu** > **Schematics**.
2. Select your workspace name. 
3. Click **Settings**. In the Summary section, your version number is displayed. 
4. Click **Update**.
5. Select a version, and click **Update**.

## Migration Sizes
Number of parallel migration will play a role of which VSI you will want to deploy with. The chart
below helps provide guidance on the VSI profile needed for the RMM server.

| Migration Size | No. of <br>Parallel Migration | VSI Profile |
| --- | :---: | :---: |
| Small | <25 | c2x4 |
| Medium | 26-50 | c4x8 |
| Large | 51-100 | c8x32 |

## Required values
| Parameters | Value | Definition |
| --- | :---: | --- |
| region | null | The MZR where the VSI is being installed. |
| VPC | null | The VPC where the VSI is being installed. |
| ssh key | null | SSH Key to access the VSI. |
| Public or Private | null | Migrate over public or private connection |
| Profile |  c2x4 | Migration size, c2x4 small, c4x8 medium, c8x32 large |
| Network | null | The subnet the VSI is being added. |
| Security group | null | The security group added to the VSI. |

## Outputs

After the resource is successfully instantiated in your IBM Cloud VPC. You will get the following
output.

| Variable Name | Description |
| --- | --- |
| resource_name | Name of the RMM VSI server. |
| IP | IP address of the RMM VSI server. |
| rmm_login | login name |
| rmm_password | password |

## Uninstalling the software

<!-- How can a user uninstall this offering? The following info is used as an example. Update
accordingly. -->

Complete the following steps to uninstall a Helm Chart from your account. 

1. Go to the **Menu** > **Schematics**.
2. Select your workspace name. 
3. Click **Actions** > **Destroy resources**. All resources in your workspace are deleted.
4. Click **Update**.
5. To delete your workspace, click **Actions** > **Delete workspace**.

## Getting support

<!-- How can a user get support for this offering? The following info is used as an example. Update
accordingly. -->

This product is provided and supported by P2V-team. If you encounter any
issues that require opening a support case, click **Get help?** at the beginning of this page to
open a GitHub issue in the corresponding repository for this chart. Your issue will typically be
answered in approximately 1 to 2 business days by the Bitnami support team.
