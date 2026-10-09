# Salesforce Administration — Hands-On Practice

## Project Overview

This repository documents my practical learning in Salesforce Administration through Salesforce Trailhead and hands-on Salesforce environments.

My work has focused on user administration, access control, security configuration, custom objects, field configuration, role hierarchy, record-level security, and sharing rules.

The purpose of this practice is to understand how Salesforce administrators configure the platform, manage user access, and implement security according to business requirements.

## 1. Salesforce Platform and Navigation

Worked with Salesforce Lightning Experience and the Setup environment to explore and configure administrative features.

Tasks and areas covered:

- Navigated Salesforce Lightning Experience and Setup.
- Used Quick Find to locate configuration settings.
- Worked with Object Manager and Salesforce administration features.
- Used hands-on Salesforce environments to perform configuration exercises.
- Navigated user management, permission settings, roles, sharing settings, and object configuration.
- Practised following business requirements and verifying configuration results.

## 2. User Administration

Performed hands-on user administration tasks in Salesforce Setup.

Work completed:

- Created Salesforce users for practice.
- Configured user-related information and account settings.
- Worked with usernames, aliases, email fields, licenses, profiles, and roles.
- Reviewed how licenses and profiles affect the permissions available to a user.
- Deactivated a test user to practise basic user lifecycle management.
- Explored the relationship between user setup and access to Salesforce features.

These exercises provided practical exposure to user provisioning and the administrative settings that influence user access.

## 3. Permission Set Configuration

Created and configured a permission set named **Manage Job Applications**.

### Object-level permissions

Configured the Job Application object with:

- Read access
- Edit access

### Field-level permissions

Configured field permissions to support the exercise's access requirements.

- Maintained Read access for the applicable fields.
- Kept Candidate and Position fields read-only.
- Enabled editing for applicable fields where required.
- Reviewed system-controlled fields for which editing was unavailable.

This exercise demonstrated how object-level permissions and field-level security work together to determine what users can access and modify.

## 4. Custom Object Creation

Created a custom object named **Referral** to practise Salesforce data modelling and record-level security.

Configuration performed:

- Object label: Referral
- Plural label: Referrals
- Record name field: Referral Name
- Record name data type: Text

This exercise provided practical exposure to creating a custom object and defining its primary record-name field.

## 5. Organization-Wide Defaults (OWD)

Configured organization-wide sharing defaults for the Referral object.

Settings configured:

- Internal access: Private
- External access: Private
- Grant Access Using Hierarchies: Disabled

The configuration was intended to restrict default record visibility and prevent automatic access through the role hierarchy for this object.

I also encountered Salesforce's sharing recalculation process after changing the sharing settings and learned why changes to organization-wide defaults may require sharing recalculation.

## 6. Role Hierarchy Configuration

Created and organized roles in the Salesforce role hierarchy.

Roles configured:

- Recruiting Manager
- Recruiter

The hierarchy was configured beneath the existing VP Human Resources role, with Recruiter reporting to Recruiting Manager.

This exercise provided hands-on experience with role creation, reporting relationships, and the role hierarchy's relationship to record access.

## 7. Custom Field and Picklist Configuration

Worked with the Program object to configure a custom field.

### Program Type

Created a picklist field named **Type** with the following practice values:

- Campus Outreach
- Development
- Research

This exercise covered custom field configuration, picklist value management, and the use of standardized selections to classify records.

## 8. Criteria-Based Sharing Rule

Created a criteria-based sharing rule named **Campus Outreach Programs**.

Configuration performed:

- Object: Program
- Rule criteria: Type equals Campus Outreach
- Shared with: Recruiter role
- Access level: Read/Write

The rule was designed to grant the specified role additional access to records matching the defined criteria.

This exercise demonstrated how sharing rules can extend record access beyond the baseline organization-wide defaults when business requirements call for it.

## 9. Salesforce Security and Access Management

Studied and practised Salesforce's layered security model through configuration exercises.

### Object-level access

Worked with permissions that determine whether a user can read or edit records of a particular object.

### Field-level security

Worked with field permissions to distinguish fields that users may view from those they may edit.

### Record-level access

Explored how organization-wide defaults, role hierarchy, and sharing rules influence access to individual records.

### Permission management

Worked with permission sets and studied how permissions can be assigned and organized according to users' responsibilities.

These areas were considered together rather than as independent settings, with attention to how the different layers affect effective access.

## 10. Permission Set Groups — Concepts Studied

Studied permission set groups as a way to combine multiple permission sets according to a job function.

Topics covered:

- Bundling permission sets into a group.
- Assigning groups according to users' responsibilities.
- Understanding the combined permissions provided by group members.
- Reusing permission sets across different access models.
- Applying the principle of least privilege.
- Understanding permission dependencies and license restrictions.
- Reviewing permission calculation and recalculation statuses.
- Using permission summaries to analyse access.
- Understanding why a user's license may restrict the permissions they can receive.

**Status:** These concepts were studied through Trailhead material and exercises. The latest recorded hands-on challenge involving the Sales Orders permission set and the Edit Activated Orders app permission was not confirmed as completed.

## 11. Business Requirements and Configuration

The practical exercises involved translating administrative requirements into Salesforce configuration.

Examples of this approach included:

- Configuring access according to an object's security requirements.
- Creating roles to represent a reporting structure.
- Using picklists to standardize record classification.
- Defining criteria for sharing selected records.
- Applying object and field permissions to control data access.
- Considering user licenses and permission dependencies when designing access.

The focus was on understanding the purpose of each configuration and verifying the result against the stated requirement.

## 12. Practical Configurations Completed

The following configurations were completed during the recorded hands-on practice:

- Created and configured Salesforce users.
- Deactivated a test user.
- Created the Manage Job Applications permission set.
- Configured Job Application object and field permissions.
- Created the Referral custom object.
- Configured Referral organization-wide defaults.
- Disabled Grant Access Using Hierarchies for Referral.
- Created Recruiting Manager and Recruiter roles.
- Configured the Program Type picklist.
- Created the Campus Outreach Programs criteria-based sharing rule.
- Configured the sharing rule to provide Read/Write access to the Recruiter role.

These items represent hands-on configuration work rather than concepts that were only studied.

## 13. Concepts Studied but Kept Separate from Completed Configurations

The following areas were covered in learning material and exercises, but are not all claimed as independently completed configurations:

- Permission set groups and combined permissions.
- Permission calculation and recalculation.
- Permission dependencies and license restrictions.
- Permission summaries and access analysis.
- Job-function-based permission assignment.
- Additional permission set group assignments and challenge-specific app permissions.

This distinction keeps the portfolio accurate about the difference between practical implementation and conceptual understanding.

## 14. Tools and Learning Environment

**Platform:** Salesforce Lightning Experience

**Learning environment:** Salesforce Trailhead and hands-on Salesforce environments

**Areas practised:** Salesforce Setup, user administration, Object Manager, permission sets, custom objects, roles, organization-wide defaults, and sharing rules.

## Technical Skills

- Salesforce Lightning Experience
- Salesforce Setup and administrative navigation
- User administration
- Profiles, licenses, and roles
- Custom objects and fields
- Picklist configuration
- Permission sets
- Object-level permissions
- Field-level security
- Organization-Wide Defaults
- Role hierarchy
- Record-level security
- Criteria-based sharing rules
- Permission set group concepts
- Least-privilege access design
- Configuration testing and verification

## Learning Outcome

Developed practical familiarity with Salesforce administration by configuring users, objects, fields, permissions, roles, and record-sharing rules in hands-on environments.

The work has strengthened my understanding of how Salesforce administrators structure data, control access, and translate business requirements into platform configuration.

**Career focus:** Entry-Level Salesforce Administrator | CRM Administrator | Salesforce Support Analyst

*Portfolio note: This repository documents self-directed Trailhead practice. It does not represent production Salesforce administration or independent implementation of configurations that are listed only as studied concepts.*
