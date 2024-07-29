{
	"info": {
		"_postman_id": "f2874495-c224-43dd-a048-efcd62533f92",
		"name": "My pet",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json",
		"_exporter_id": "24272038"
	},
	"item": [
		{
			"name": "Сreating an animal",
			"event": [
				{
					"listen": "test",
					"script": {
						"exec": [
							"pm.test(\"Status code is 200\", function () {\r",
							"    pm.response.to.have.status(200);"
						],
						"type": "text/javascript"
					}
				}
			],
			"request": {
				"method": "POST",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n  \"id\": 790,\r\n  \"category\": {\r\n    \"id\": 777,\r\n    \"name\": \"armenian gampr\"\r\n  },\r\n  \"name\": \"Jambo\",\r\n  \"photoUrls\": [\r\n    \"https://vstrokax.net/wp-content/uploads/2021/10/vne_strok_om.jpg\"\r\n  ],\r\n  \"tags\": [\r\n    {\r\n      \"id\": 0,\r\n      \"name\": \"string\"\r\n    }\r\n  ],\r\n  \"status\": \"available\"\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://petstore.swagger.io/v2/pet/",
					"protocol": "https",
					"host": [
						"petstore",
						"swagger",
						"io"
					],
					"path": [
						"v2",
						"pet",
						""
					]
				}
			},
			"response": []
		},
		{
			"name": "Сhecking the Armenian gampra",
			"event": [
				{
					"listen": "test",
					"script": {
						"exec": [
							"pm.test(\"Status code is 200\", function () {\r",
							"    pm.response.to.have.status(200);\r",
							"});"
						],
						"type": "text/javascript"
					}
				}
			],
			"protocolProfileBehavior": {
				"disableBodyPruning": true
			},
			"request": {
				"method": "GET",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "\r\n  \"id\": 790,\r\n  \"category\": {\r\n    \"id\": 777,\r\n    \"name\": \"armenian gampr\"\r\n  },\r\n  \"name\": \"Jambo\",\r\n  \"photoUrls\": [\r\n    \"https://vstrokax.net/wp-content/uploads/2021/10/vne_strok_om.jpg\"\r\n  ],\r\n  \"tags\": [\r\n    {\r\n      \"id\": 0,\r\n      \"name\": \"string\"\r\n    }\r\n  ],\r\n  \"status\": \"available\"\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://petstore.swagger.io/v2/pet/790",
					"protocol": "https",
					"host": [
						"petstore",
						"swagger",
						"io"
					],
					"path": [
						"v2",
						"pet",
						"790"
					]
				}
			},
			"response": []
		},
		{
			"name": "Update create user",
			"event": [
				{
					"listen": "test",
					"script": {
						"exec": [
							"pm.test(\"Status code is 200\", function () {\r",
							"    pm.response.to.have.status(200);\r",
							"});"
						],
						"type": "text/javascript"
					}
				}
			],
			"request": {
				"method": "PUT",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n  \"id\": 7900,\r\n  \"category\": {\r\n    \"id\": 777,\r\n    \"name\": \"armenian gampr\"\r\n  },\r\n  \"name\": \"Jeak\",\r\n  \"photoUrls\": [\r\n    \"https://vstrokax.net/wp-content/uploads/2021/10/vne_strok_om.jpg\"\r\n  ],\r\n  \"tags\": [\r\n    {\r\n      \"id\": 0,\r\n      \"name\": \"string\"\r\n    }\r\n  ],\r\n  \"status\": \"available\"\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://petstore.swagger.io/v2/pet/",
					"protocol": "https",
					"host": [
						"petstore",
						"swagger",
						"io"
					],
					"path": [
						"v2",
						"pet",
						""
					]
				}
			},
			"response": []
		},
		{
			"name": "Сhecking Update ",
			"event": [
				{
					"listen": "test",
					"script": {
						"exec": [
							"pm.test(\"Status code is 200\", function () {\r",
							"    pm.response.to.have.status(200);\r",
							"});"
						],
						"type": "text/javascript"
					}
				}
			],
			"request": {
				"method": "GET",
				"header": [],
				"url": {
					"raw": "https://petstore.swagger.io/v2/pet/7900",
					"protocol": "https",
					"host": [
						"petstore",
						"swagger",
						"io"
					],
					"path": [
						"v2",
						"pet",
						"7900"
					]
				}
			},
			"response": []
		},
		{
			"name": "Delete the Armenian gampr",
			"event": [
				{
					"listen": "test",
					"script": {
						"exec": [
							"pm.test(\"Status code is 200\", function () {\r",
							"    pm.response.to.have.status(200);\r",
							"});"
						],
						"type": "text/javascript"
					}
				}
			],
			"request": {
				"method": "DELETE",
				"header": [
					{
						"key": "api_key",
						"value": "special-key",
						"type": "text"
					}
				],
				"url": {
					"raw": "https://petstore.swagger.io/v2/pet/790",
					"protocol": "https",
					"host": [
						"petstore",
						"swagger",
						"io"
					],
					"path": [
						"v2",
						"pet",
						"790"
					]
				}
			},
			"response": []
		},
		{
			"name": "Check deleted",
			"event": [
				{
					"listen": "test",
					"script": {
						"exec": [
							"pm.test(\"Status code is 200\", function () {\r",
							"    pm.response.to.have.status(200);\r",
							"});"
						],
						"type": "text/javascript"
					}
				}
			],
			"request": {
				"method": "GET",
				"header": [],
				"url": {
					"raw": "https://petstore.swagger.io/v2/pet/790",
					"protocol": "https",
					"host": [
						"petstore",
						"swagger",
						"io"
					],
					"path": [
						"v2",
						"pet",
						"790"
					]
				}
			},
			"response": []
		}
	]
}
