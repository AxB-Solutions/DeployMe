# DeployMe

# Basic Premis

An easier way for teams to manage deployments between salesforce orgs.
- Reliable
- robust
- intelligent - understands sf metadata structure and alerts of issues before they occur

# Dependency notes
deployment process:
- labels
	- no dependencies. Other components depend on labels
- global value sets
	- no dependencies. Other components depend on value sets
- roles
	- no dependencies
- standard value sets
	- field must exist. Standard fields always exist
- custom permissions
	- no dependencies
- groups
	- users
- queues
	- groups
	- users
- custom objects
	- objects fields may reference other objects
	- validation rules depend on object fields
	- record types depend on picklist values
	- list views depend on fields
	- field sets depend on fields
	- picklist fields have their own set of dependencies
			- picklist values cannot be duplicated
			- dependent picklist fields - values must exist on parent or child
	- lookup fields
		- other object must exist
- tabs
	- require the object to exist
- permission sets
	- fields for object must exist
	- connected apps must exist
	- custom permissions must exist
- apex
	- objects and fields
	- other classes
	- custom labels
	- metadata objects
- pages
	- require the apex class to exist
- apex components
	- require the apex class to exist
- triggers
	- require the apex class to exist
	- objects and fields
- aura
	- require the apex class to exist
	-
- lwc
	- apex classes
	- object fields
- flows
	- apex classes
	- object fields
	- groups
	- emails
	- alerts
	- permission sets
	- custom labels
	- aura components
	- lwc components
- quick actions
	- object
	- lwc
	- aura
	- flow
- flexi pages
	- fields
	- object
	- layout
	- custom permissions
- custom metadata
	- custom metadata fields and object