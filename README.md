# Nerofy metadata repository
This repository provides JSON metadata, such as updates and links (etc.), for Nerofy projects and services
## Additional information

- Within the repository itself, there is no additional content. Images, videos, and other files are hosted separately. This repository is solely for providing metadata and links to the related files.
- Furthermore, the metadata repository does not contain any security-relevant information. Personal data, configurations, and other sensitive data are processed independently by the respective services and are not publicly stored in this repository.
## Usage

The metadata within this repository is free to use and unlicensed. However, please be aware that this only applies to this meta repository. The linked content may have its own licenses and copyright terms, thus this repository cannot grant rights of use for the linked data.


## Service endpoints

Theoretically, this repository can serve as an API endpoint since it responds exclusively in JSON format. However, please do not access this repository directly; instead, self-host the data as your own endpoint or use our official meta endpoint `https://meta.nrfy.net/`.

#### Service overview

```http
  GET /services/
```

#### Get metadata root for a specific service

```http
  GET /services/${service.id}/
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `service.id`      | `string` | **Required**. The id of the Nerofy service (e.g: nexus-app) |
