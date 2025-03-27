# Messages Schemas

## Introduction

In Kanvas Social we use Messages as Posts in a Social Media Scenario. Every Message has a a type `Message_Type` 
in which a message schema is defined. This schema serves as contract for how the incoming data will be structured and conforms to Laravel's data validation feature.


## The Structure
 
Here is an example:

```json
{
		"title": "required|string",
		"nugget": "required|string",
		"ai_model": "required|array",
		"description": "required|string",
		"ai_model.key": "required|string",
		"ai_model.name": "required|string",
		"ai_model.value": "required|string",
		"ai_model.payment": "required|array",
		"ai_model.payment.price": "required|integer",
		"ai_model.payment.is_locked": "required|boolean",
		"ai_model.payment.free_regeneration": "required|boolean"
}
```

For more information about this structure take a look at [Laravel's Validation](https://laravel.com/docs/11.x/validation#introduction) feature. This pretty much works the same as that.

