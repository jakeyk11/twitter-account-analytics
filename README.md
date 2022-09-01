# Twitter Account Analytics
This repository contains a data collection routine and front-end to monitor and analyse activity for a chosen twitter account.

## Contents

<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#project-description"> ➤ Project Description </a></li>
    <li><a href="#folder-structure"> ➤ Folder Structure</a></li>
    <li>
      <a href="#setup-and-usage"> ➤ Setup and Usage</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
  </ol>
</details>

## Project Description

## Folder Structure

    twitter-account-analytics
    │
    ├── ml_algorithms
    │   ├── __init__.py
    │   ├── k_means.py    
    │   ├── k_nearest_neighbours.py
    │   ├── linear_regression.py
    │   ├── mean_shift.py
    │   ├── support_vector_machine.py
    │ 
    ├── get_account_activity.py 
    │
    ├── LICENSE 
    │ 
    ├── README.md 

## Setup and Usage

### Prerequisites

<li> Twitter API Essential Access - <a href="https://developer.twitter.com/en/docs/twitter-api?utm_source=advocacy&utm_medium=organic&utm_campaign=signup"> Sign up here. </a></li>
<li> A single app and project created within the <a href="https://developer.twitter.com/en/portal/dashboard">Developer Portal Dashboard</a></li>

### API Keys and Environment Variables

When setting up an app and project within the Developer Portal, a number of API keys/tokens will be made available. These should be noted down and stored as environment variables. The environment variables should be set using the following convention (Windows):

    set TWITTER_CONSUMER_KEY='<Insert your consumer API key>'
    set TWITTER_CONSUMER_SECRET='<Insert your consumer API secret>'
    set TWITTER_BEARER_TOKEN='<Insert your bearer token>'
    set TWITTER_ACCESS_TOKEN='<Insert your access token>'
    set TWITTER_ACCESS_SECRET='<Insert your access secret>'

Remember to replace the contents of <code>< ></code> with your credentials (remove the <code>< ></code>). Credentials must be enclosed in single quotation marks as shown above.

### Temporary info

The following open source packages are used in this project:
* Numpy
* Matplotlib
* Scikit-Learn
* Random
* Warnings
* Collections
* Sys
* OS

The ML algorithms that have been developed are contained within a package named <a href="https://github.com/jakeyk11/ml-algorithms-from-scratch/tree/main/ml_algorithms">ml_algorithms</a>. Given that the package has not yet been formally deployed, it is advised that the user takes the following steps:
<ol>
  <li>Clone the project and save to a local area</li>
  <li>Add the ml_algorithms directory to the environment path</li>
  <li>Import the required machine learning algorithm</li>
</ol>

For example, to load the linear regression algorithm when working within the <a href="https://github.com/jakeyk11/ml-algorithms-from-scratch/tree/main/model_testing">model_testing</a> directory, the following code may be written within Python:

    import os
    import sys
    root_folder = os.path.abspath(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
    sys.path.append(root_folder)
    
    from ml_algorithms.linear_regression import LinearRegression

For convenience, the project directory contains an area to store data (<a href="https://github.com/jakeyk11/ml-algorithms-from-scratch/tree/main/datasets">datasets</a>) and an area to test ML algorithms (<a href="https://github.com/jakeyk11/ml-algorithms-from-scratch/tree/main/model_testing">model_testing</a>).
