# AEM Crawler | Automation Tool

###### Timeline | 2016-17 (Internship - Dell International Services India Pvt. Ltd.)

During my Summer Internship 2017 with DELL, I was assigned a project where I developed a full fledged Windows Desktop application using JavaFX to address the concerned challenges. In the organization, developer spends x amount of time on updating a page, while a quality reviewer spends x+1 amount of time to perform the quality check on the same page. **AEM crawler** is an endeavor to reduce the time spent on peer reviewing the pages. The team wanted a solution which would automate the task of quality check which involved 28 checklist points to be covered. After developing any page on www.dell.com they have to undergo manual quality review check for those 28 checklist points, which needed lots of manual effort and is prone to frequent errors. But using the developed tool the whole process was automated with almost all checklist points covered and then hunderds of hours of work is reduced to only few minutes.

## Demonstration

![](/Windows%20App%20|%20AEM%20Crawler/AEM-Crawler.gif)

###### This tool has many other complex functionalities integrated. Due to company privacy and NDA, just showcasing the overview look of the working tool.


## Methodology
AEM Crawler is an Automated Audit Tool, exclusively built for the applications on **[AEM (Adobe Experience Manager) Content Management System](https://www.adobe.com/in/marketing/experience-manager-sites.html)**. It is a Java based Windows Desktop Application developed using JavaFX and FXML technologies on the Eclipse IDE. This tool requires the reviewer to input the site URL that has to be reviewed. Input can be a list of multiple URLs or any number of URLs in an excel sheet. Using the SSO sign in on AEM CMS it crawls the provided sites and reviews the desired resources. The generated review data by the tool can be extracted as output in Excel sheets. AEM Crawler is loaded with multiple features for:

- Extraction of reference URLs
- Asset details extraction
- Page Component list
- Referred URL verification
- Page content validation

This tool has following modules implemented that perform the required review of the sites and cover almost all of the 28 checklist review points as required by the business.

**URL Extractor**
1. Helps in pulling all the URLs referred inside the given page
2. Distinguish page as Auth/UnAuth & internal/external

**Page Content Audit**
1. Provides Component details with Name and Content along with the required word/phrase replacement
2. Verifies page layout control
3. Validates link reference, extension, functionality and localized PDFs

**Asset Extractor** - Generates list of Images, PDFs, docs and all other assets available on the page

**Components Audit** - Obtain the list of all components that are made use on the page along with the respective content and related CTA IDs

## Technology Stack
- Languages	|	JavaFX and FXML
- IDE	| Eclipse and FX Scene Builder
- Database | Microsoft Excel
- Graphics Design	|	Adobe Photoshop CS6

## Implemented Concepts
- [Apache POI - the Java API for Microsoft Documents](https://poi.apache.org/)
- [JavaFX Scene building using Gluon Scene Builder ](https://gluonhq.com/products/scene-builder/)
- HttpURLConnection Package
- WebEngine and WebView Class
- CSS for designing the table layouts
- Java IO File manipulation
- JavaFX EventHandler Class 
- Observable List and FXCollections
- Different Scene Controls
	- ListView
	- TableView
	- ComboBox
	- File Chooser
	- Alert Dialog
	- ProgressIndicator and ProgressBar
	- Concurrent Task
	- Model/Bean Classes for table data
	- Preferences
	- Map, HashMap, ArrayList
- Graphics Design | Image and Icon editing, refactoring
