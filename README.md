# Machine Learning Engineer Nanodegree - Udacity

## Supervised Learning

### Project: Capstone Project - Predicting the customer churn for a Brazilian Newspaper Media

####  Install

This project requires Python 3.6 and the following Python libraries installed:

    NumPy
    Pandas
    matplotlib
    scikit-learn
    seaborn
    time
    datetime

You will also need to have software installed to run and execute an iPython Notebook (jupyter-notebook, for instance)

We recommend to install Anaconda, a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.

#### Code

Code is provided in the CapstoneFinalProject.ipynb notebook file. It uses the completesubscribers06.csv, canceledsubscriberscomplete06.csv, and Cancelamentos 062018.xlsx dataset files. Code uses all the libraries mentioned above. Code uses classification technique of Supervised Learning to train the model and Unsupervised Learning to balance the dataset. Code has implemented ADABoost Classifier, Gradient Descent Classifier, and Random Forest Classifier. Code also has an implementation of the benchmark model (RFV model).

#### Run

In a terminal or command window, navigate to the top-level project directory capstone_project/ (that contains this README) and run one of the following commands:


```python
ipython notebook CapstoneFinalProject.ipynb
```

or


```python
jupyter notebook CapstoneFinalProject.ipynb
```

This will open the iPython Notebook software and project file in your browser.


#### Data

The datasets to be used in the project were provided by GP and contains browsing histories of users. Information such as how the dataset was obtained, and the characteristics of the dataset should be included as well. Basically, there will be two datasets. Both of them containing data for the month of June. There will be one dataset consisting of browsing history of people who did not practice the churn and the other one consisting of browsing history of people who did practice the churn. The features contained in all datasets are listed and explained bellow:

- **Subscription_id**: An *id* to identify an user at the database;
- **type**: *T* for titular account and *D* for dependent account member;
- **Recency**: A variable that varies from 0 to 30. It measures how recent a user have visited the website, where 0 means that he never had visited in the last 30 days and 30 that he came yesterday;
- **last_access_date**: Last day of user's access at the website;
- **lst_date**: a string containing all the days that the user have accessed the website;
- **subscription_date**: the precise day that the user have subscribed;
- **freq**: How many days the user have visited the website;
- **qt_page_view**: quantity of page views a user has;
- **qt_page_view_week**: quantity of page views during the weeks;
- **qt_page_view_weekend**: quantity of page views during the weekends;
- **qt_page_view_mornig**: quantity of page views during the mornings;
- **qt_page_view_afternoon**: quantity of page views during the afternoons;
- **qt_page_view_nigth**: quantity of page views during the nights;
- **qt_art_read**: quantity of articles that were read by a user;
- **qt_source_sm_cpc_facebook**: how many times a user came to the website via a paid campaign from facebook;
- **qt_source_sm_cpc_others**: how many times a user came to the website via a paid campaign from others social medias;
- **qt_source_sm_cpc_others**: how many times a user came to the website via a paid campaign from others social medias;
- **qt_source_sm_facebook**: how many times a user came to the website via facebook (no paid campaign);
- **qt_source_sm_other**: how many times a user came to the website via other social media (no paid campaign);
- **qt_source_nedeal**: how many times a user came to the website via actions from a outsourced;
- **qt_source_email**: how many times a user came to the website via a mail list;
- **qt_source_others**: how many times a user came to the website via other source;
- **qt_gazeta_capa**: how many times a user accessed the website front page;
- **qt_gazeta_esportes**: how many times a user accessed the website section "esportes";
- **qt_gazeta_politica**: how many times a user accessed the website section "politica";
- **qt_gazeta_economia**: how many times a user accessed the website section "economia";
- **qt_gazeta_curitiba**: how many times a user accessed the website section "curitiba"; 
- **qt_agronegocio**: how many times a user accessed the website section "agronegocio";
- **qt_haus**: how many times a user accessed the website section "haus";
- **qt_bom_gourmet**: how many times a user accessed the website section "bom gourmet";
- **qt_viver_bem**: how many times a user accessed the website section "viver bem";	
- **qt_guia**: how many times a user accessed the website section "guia";	
- **qt_access_others**: how many times a user accessed other pages of the website;
- **qt_comments**: how many times a user have made some comment at the website comment section;
- **qt_explicar**: how many times a user have read some article with the tag "explicar";
- **qt_alegre**: how many times a user have read some article with the tag "alegre";
- **qt_provocar**: how many times a user have read some article with the tag "provocar";
- **qt_triste**: how many times a user have read some article with the tag "triste";
- **qt_inspirar**: how many times a user have read some article with the tag "inspirar";
- **qt_moderno**: how many times a user have read some article with the tag "moderno";
- **qt_facilitar**: how many times a user have read some article with the tag "facilitar";
- **qt_surpreendente**: how many times a user have read some article with the tag "surpreendente";
- **qt_informar**: how many times a user have read some article with the tag "informar";
- **qt_hardnews**: how many times a user have read some article with the tag "hardnews";
- **qt_softnews**: how many times a user have read some article with the tag "softnews";
- **qt_appGazeta**: how many times a user have used the app section "gazeta" to access the website;
- **qt_appGuia**: how many times a user have used the app section "guia" to access the website;
- **qt_mobile**: how many times a user have used a mobile to access the website;
- **qt_other_devices**: how many times a user have used other devices rather than mobile to access the website;
- **qt_login**: how many times a user have logged in;
- **browser**: the user most common used browser to access the website;
- **has_club**: if the user has club, which is another product of the newspaper media;
- **has_print**: if the user has a printed version of the newspaper;
- **Churn**: the output variable; if the user practiced the Churn or not (target variable).

The dataset contains $62581$ data points, where $1371$ data points for the class of people who did practice the churn and $61210$ who didn't and it is divided in three files:

- 'subscriberscomplete06.csv' -- It contains all the payed subscribers that, at the end of June, did not cease to be a payed subscriber; 
- 'canceledsubscriberscomplete06.csv' -- It contains all the payed subscribers that, at the end of June, ceased to be a subscriber;
- 'Cancelamentos 062018.xlsx' -- It contains the list of all the subscribers that ceased to be a payed subscriber at the end of June, but with a column specifying if the user stopped the payment voluntarily or because of financial issue that forced the company to cut off the subscriber from the payed subscribers list.
