When an organization node contains lots of folders, projects, and resources, a workforce 
might need to restrict who has access to what
To help with this task, administrators can use Identity and Access Management, or IAM.

With IAM, administrators can apply policies that define **who** can do **what** and on **which** resources.

The “**who**” part of an IAM policy can be: 
● a Google account, 
● a Google group, 
● a service account, or 
● a Cloud Identity domain. 
A “who” is also called a “principal.” Each principle has its own identifier, usually an email address.

The “can do what” part of an IAM policy is defined by a role. 
**An IAM role is a collection of permissions.** When you grant a role to a principal, you grant all the permissions that the role contains.

- You can define deny rules that prevent certain principals from using certain permissions, regardless of the roles they're granted. 
- This is because IAM always checks relevant deny policies before checking relevant allow policies. 
- Deny policies, like allow policies, are inherited through the resource hierarchy.

There are three kinds of roles in IAM: basic, predefined, and custom.

The first role type is basic. Basic roles are quite broad in scope. When applied to a Google Cloud project, they affect all resources in that project.

Basic roles include 
- owner, 
- editor, 
- viewer, and 
- billing administrator. 
Let’s look at these basic roles in a bit more detail.

- Project viewers can access resources but can’t make changes. 
- Project editors can access and make changes to a resource. 
- And project owners can also access and make changes to a resource. In addition, project owners can manage the associated roles and permissions and set up billing. 
- Often companies want someone to control the billing for a project but not be able to change the resources in the project. This is possible through a billing administrator role.