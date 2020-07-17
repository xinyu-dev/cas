# My Volunteer Projects at the Chinese Antibody Society
Resources and templates I made for CAS

# AWS S3 Hosted Playground, Distributed through CloudFront

Created [this playground website](http://chineseantibody-dev.org/) on AWS S3 is a collection of static webpages currently under development for a future version of [the society's website](https://chineseantibody.org/). Domain name was purchased through AWS Route 53, website files hosted on AWS S3, SSL certificate obtainted through AWS Certificate Manager, and website distributed through AWS CloudFront

# AWS EC2 IPython (Jupyter Notebook) Cloud Computation Environment

Created this cloud computation environemnt in AWS EC2 for hosting python scripts. Notebook can be [accessed here](https://ec2-18-217-92-114.us-east-2.compute.amazonaws.com:8888/tree/MyNotebooks/). *To access the link, you need to be authorized by the opertional team of the Chinese Antibody Society*.

# Django Application (Volunteer Hub) Deployed on Elastic Beanstalk

Created a Django application for the [CAS volunteer hub](https://hub.chineseantibody-dev.org). Deployed on Elastic Beanstalk


# Collection of Scripts and Templates (2020)

## Python - Image Processing (All scripts hosting on CAS's AWS EC2 cloud)

### 1. Logo Resizer (code in separate [repo](https://github.com/xinyu-dev/general-image-processing))

Batch-transform sponsor logos to uniform dimensions without shape distortion.

## Python - Retrieving data from APIs 

*Note: you need to be authorized by the Chinese Antibody Society to receive API tokens*.  

### 1. Using MailChimp API to retrieve stats on email campaigns

The script retrieves these data fields: 

```python
campStats={
    'article_type':[],
    'send_time':[],
    'list_name':[],
    'subject_line':[],
    'emails_sent':[],
    'bounces':[],
    'unsubscribed':[],
    'open_total':[],
    'unique_opens':[],
    'clicks_total':[],
    'unique_clicks':[],
    'ind_open_rate':[],
    'ind_click_rate':[],
    'ind_unsub_rate':[]
}
```

### 2. Using CloudFlare API to retrieves stats on website traffic

The script retrieves these data fields: 

```python
webStats={
    'date_time':[],
    'requests_all':[],
    'requests_country':[],
    'threats_all':[],
    'pageviews_all':[],
    'unique_visitors':[]
}
```

## Python - Analytics Dashboard

The data retrieved from the APIs using the scripts above can be consumed directly by a Dash/Plotly app that I built. The analytics app is currently hosted on Heroku. 


## HTML, Javscript, CSS

### 1. Email newsletter for journal new article alert

 - Code : `New Article Alert.html`
 - [Demo](https://xinyu-dev.github.io/cas/New%20Article%20Alert.html)
 
### 2. Email newsletter for journal announcements

 - Code : `News and Announcement.html`
 - [Demo](https://xinyu-dev.github.io/cas/News%20and%20Announcement.html)

### 3. CAS Program Book, embedded in Adobe InDesign (original artworks made in Adobe InDesign)

 - Code : `CAS Program Book.html`
 - [Demo](https://xinyu-dev.github.io/cas//CAS%20Program%20Book.html)

### 4. Interactive Webinar Database (code in a seprate [repo](https://github.com/xinyu-dev/interactive-datatable))
 - Version 1: Expandable dropdown menu for each row to hide certain user-defined columns.
   - [Table Only Demo](https://xinyu-dev.github.io/interactive-datatable/webinar_v1.html)

 - Version 2: Responsive to screen size. Automatically hide whatever number of rows needed. 
   - [Table Only Demo](https://xinyu-dev.github.io/interactive-datatable/webinar_v2.html) 
   - [Table in a themed page](http://chineseantibody-dev.org/webinar-test.html)

### 5. Filterable Sortable, and Searchable Video-Embedded Webinar Database
  Modified javascript & HTML based on isotype.js and booststrap to enable embedding of video iframes in Boostrap cards. These cards be be filtered, sorted, and searched by text. 
  - [Demo](https://s3.us-east-2.amazonaws.com/chineseantibody-dev.org/webinar-past.html) 
      
