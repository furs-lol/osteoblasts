---
sidebar_position: 1
---

### **GET** `/users/me`

Gets the current authenticated user

#### Example Response

```json
{
	"Id": 1,
	"Username": "ibx34",
	"Dob": "2000-06-17T00:00:00Z",
	"Bio": null,
	"Pronouns": null,
	"Sexuality": null,
	"Avatar": null,
	"Banner": null,
	"Gender": null,
	"TwoFactor": false,
	"PublicFlags": 0,
	"Verified": false,
	"Email": "noreply@furs.lol"
}
```

---

### **GET** `/users/me/posts`

Gets the authenticated user's posts.

#### Example Response

```json
[
	{
		"Author": {
			"Id": 1,
			"Username": "ibx34",
			"PublicFlags": 0,
			"Avatar": null,
			"Banner": null
		},
		"Id": "Fn-7AcxKM5SHCK3iQt88G",
		"Hash": "totally-real-file-hash",
		"Title": "Screenshot",
		"Description": null,
		"CreatedAt": "2022-07-28T22:30:39.845681Z",
		"Flags": 0,
		"Tags": null
	}
]
```


---

### **GET** `/users/{user.id}`

Gets the requested user. If the requested user's profile is marked NSFW the user requesting them must be above the age of 18.
This route does not require authentication, in most cases. If the requested user's profile is private, or NSFW it will require
the user requesting the user is authenticated.