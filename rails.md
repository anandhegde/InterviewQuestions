1. **update_attribute vs update_attributes**

	- update_attribute is for updating single attribute and it doesnot check the validation. In rails4 onwards we can use Model.update_column(:column, value)
	- update_attribtues is for multiple argumetns and checks the validation

2. Callbacks in rails (in Active Record)
	- methods which get called during the life cycle of an object
	- methods can be called whenever an object is created, updated, deleted, saved, validated or loaded from database.
	- Here is a list with all the available Active Record callbacks, listed in the same order in which they will get called during the respective operations:

		**Creating an Object**
		- before_validation
		- after_validation
		- before_save
		- around_save
		- before_create
		- around_create
		- after_create
		- after_save
		- after_commit/after_rollback
		**Updating an Object**
		- before_validation
		- after_validation
		- before_save
		- around_save
		- before_update
		- around_update
		- after_update
		- after_save
		- after_commit/after_rollback
		**Destroying an Object**
		- before_destroy
		- around_destroy
		- after_destroy
		- after_commit/after_rollback
