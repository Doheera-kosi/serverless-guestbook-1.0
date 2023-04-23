# Serverless Guestbook

<!-- TABLE OF CONTENTS -->

# 📗 Table of Contents

- [📖 About the Project](#about-project)
  - [🛠 Built With](#built-with)
    - [Tech Stack](#tech-stack)
    - [Key Features](#key-features)
  - [🚀 Live Demo](#live-demo)
- [💻 Getting Started](#getting-started)
  - [Setup](#setup)
  - [Prerequisites](#prerequisites)
  - [Install](#install)
  - [Usage](#usage)
  - [Run tests](#run-tests)
  - [Deployment](#deployment)
- [👥 Authors](#authors)
- [🔭 Future Features](#future-features)
- [🤝 Contributing](#contributing)
- [⭐️ Show your support](#support)
- [🙏 Acknowledgements](#acknowledgements)
- [❓ FAQ (OPTIONAL)](#faq)
- [📝 License](#license)

<!-- PROJECT DESCRIPTION -->

# 📖 Serverless Guestbook <a name="about-project"></a>

**Serverless Guestbook** is a simple guestbook website where users can post messages. The website is hosted in two different ways using the serverless and microservices architecture. One version uses object storage to host the site's files and the other deploys the static website as a microservice on Red Hat OpenShift.

## 🛠 Built With <a name="built-with"></a>

### Tech Stack <a name="tech-stack"></a>

<details>
  <summary>Frontend</summary>
  <ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
  </ul>
</details>

<details>
  <summary>Backend</summary>
  <ul>
    <li>Node.js</li>
    <li>Express.js</li>
  </ul>
</details>

<details>
<summary>Database</summary>
  <ul>
    <li>AWS DynamoDB</li>
  </ul>
</details>

<details>
<summary>Hosting</summary>
  <ul>
    <li>Red Hat OpenShift</li>
    <li>AWS S3 Bucket</li>
  </ul>
</details>


### Key Features <a name="key-features"></a>

- **Guestbook form:** Allows users to submit their name and message
- **API endpoint:** Exposes a REST API to store and retrieve guestbook messages
- **Static website hosting:** The website is hosted in AWS S3 bucket
- **Microservices deployment:** The website is deployed as a microservice on Red Hat OpenShift

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LIVE DEMO -->

## 🚀 Live Demo <a name="live-demo"></a>

- [OpenShift Live Link](http://serverless-guestbook-1-0-sn-labs-kupourevans9.labs-prod-openshift-san-a45631dc5778dc6371c67d206ba9ae5c-0000.us-east.containers.appdomain.cloud/)
- [AWS S3 Live Link](https://ican-guestbook.s3-web.eu-de.cloud-object-storage.appdomain.cloud/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->

## 💻 Getting Started <a name="getting-started"></a>

### Prerequisites

In order to run this project, you need:

- Node.js installed on your local machine
- An IBM Cloud account to use Object Storage and OpenShift

### Setup

Clone this repository to your desired folder:

```sh
  git clone https://github.com/Doheera-kosi/serverless-guestbook.git
```

Navigate to the project directory:

```sh
  cd serverless-guestbook
```

Install the required dependencies:

```sh
  npm install
```

### Usage

To run the project locally, you need to provide your own IBM Cloud Object Storage and OpenShift credentials as environment variables. To do this, create a `.env` file in the root directory of the project and add the following lines, replacing the placeholders with your actual credentials:

```sh
  IBM_API_KEY=<your_ibm_cloud_api_key>
  IBM_COS_ENDPOINT=<your_ibm_cloud_cos_endpoint>
  IBM_COS_BUCKET=<your_ibm_cloud_cos_bucket>
  IBM_COS_REGION=<your_ibm_cloud_cos_region>
  IBM_OPENSHIFT_URL=<your_ibm_cloud_openshift_url>
  IBM_OPENSHIFT_TOKEN=<your_ibm_cloud_openshift_token>
```

Then, run the project:

```sh
  npm start
```

Open your browser and navigate to `http://localhost:3000` to view the guestbook.

### Deployment

To deploy the project on IBM Cloud Object Storage and OpenShift, follow the steps below:

1. Make sure you have created the `.env` file with your IBM Cloud Object Storage and OpenShift credentials (as described above).

2. Build the project for deployment:

```sh
  npm run build
```

3. Deploy the project:

```sh
  npm run deploy
```

This will deploy the static website on IBM Cloud Object Storage and the REST API on OpenShift.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- AUTHORS -->

## 👥 Authors <a name="authors"></a>

This project was created by:

👤 **Evans Kupour**

- LinkedIn: [LinkedIn](https://www.linkedin.com/in/linkin-evans/)
- GitHub: [@Doheera-kosi](https://github.com/Doheera-kosi)
- Twitter: [@KupourE](https://twitter.com/@KupourE)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- FUTURE FEATURES -->

## 🔭 Future Features <a name="future-features"></a>

- **[future_feature_1]**
- **[future_feature_2]**
- **[future_feature_3]**

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->

## 🤝 Contributing <a name="contributing"></a>

Contributions, issues, and feature requests are welcome!
Feel free to check the [issues page](../../issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- SUPPORT -->

## ⭐️ Show your support <a name="support"></a>

Give a ⭐️ if you like this project!

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGEMENTS -->

## 🙏 Acknowledgements <a name="acknowledgements"></a>

- [OpenShift](https://www.openshift.com/)
- [IBM Cloud Object Storage](https://www.ibm.com/cloud/object-storage)

<p align="right">(<a href="#readme-top">back