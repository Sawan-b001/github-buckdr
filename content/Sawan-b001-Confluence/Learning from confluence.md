### EU Pro Card Process

Read about the flow of Twikey Signing Mechanism for NL, BE, FR and the Test Data for every region including proudct data and Signing Data for Pro Card

## Pull Request

Read about the Conditions to check before creating a PR and While Reviewing the PR. How a PR Should be check before Merging
#### Before Creating a PR

1. Have merged the latest copy of Develop fist
2. check for difference for anything that can accidently commited to the branch
- look out for files that should not be in commit but can be in the   git igonre file
3. Have followed all coding standards
- Appropropriate functions/class/etc names
- Code has been annotated commented where applicable
4. if necessary update readme file
5. test have been added/updated to reflect acceptance criteria
6. All existing and new tests are passing locally
7. Check dependancy have been added correctly 

#### When creating a PR

- Add any additional testing steps/guide beyond what is defined in the ticket
- Add any other dependancies (e.g branches and PRs) to the description of the PR being opened
- If lots of changes have been made, adding an explanation of why can be helpful if you have had to do something for a specific reason.his saves time and means the person reviewing won't have to ask questions
- Add screenshots of changes (where appropriate)
- If specific reviewers are required they can be assigned, but don't need to be - everyone should be reviewing PRs

##### When reviewing a PR

- Follow the same checks you would make when creating a pull request
- Small PRs can be merged once one person has approved
- Larger PRs can be merged once two people have approved (and all tests are passing)
- When merging (and moving ticket to done) Ensure the release version is added to the ticket
- Add any translation updates to the release page in Confluence
- Add any env/config change requirements to the release page

### Definition of Done

All the points which are listed must be passed like there must be no reproducable bug, QA Tested all nd all the criteria must be passed to.

### EU App releases

### UK App releases


### Process to release mew version of the App

Prepare release candidate branch
Build and deploy the app to TestFlight/Play Store
Updated release notes on the App Stores listings
Updated any necessary app listing with new info
Submit to Apple/Google for a review
If the app was approved then schedule or release the build to public
If not approved, resolve all problems and repeat from step 1
Monitor Crashlytics and Datadog for 3 to 7 days

### Coding guidenlines and Shared Codebase

**Problem :** the app shares a single codebase and different regions can benefit from the development of other regions, the requirements of some of the features or designing is not always 100% aligned

 - Read About the proposed workflow 
 - Code Architecture  
 - UI Code Architecture
 - Code Review


 ### Bloomreach Prodcuts Recommendation

 ##### Bloomrach widget 
 The Widget Configurator is a functionality within the Bloomreach Dashboard that allows you to create and manage the Recommendations and Pathways widgets easily. we can create, delete, manage, change the widget type according to our need of services.
 In Toolstation we are using following bloomreach widgets like:

 top_seller_id
 recommended_home_id
 recommended_products_id
 _fallback_recommended_id

 - APi
 - Widgets ID's Currently in use there App locations, Name, Widget ID, Widget Param, searcserviceMethdo

 ### Bloomreach Product search

 curent imlemented functionality

 - can suggest products along with queries in your autosuggest API calls. When a visitor to your site begins typing a query, the autosuggest call retrieves a text-based list of queries as well as products. By default, the response includes a maximum of eight products.

- Input String
- Request
- Output
- API Rsponse
-  **PLP In Stock** 

### Next Day Collection 

Next Day Collection allows a customer to order items for collection on the next business day from their favourite brach if there is currently insufficient stock at the brach for a same day collection. This allows customers access to delivery stock without having to pay for delivery.

- Trolley 
- Cut-Off Time Messages
- SWITCHING FROM DELIVERY
- Order History
- Saved Lists


## Content Square

Contentsquare is basically used for Analytics. it is an SDK in the mobile app, Contentsquare anonymously tracks all mouse movements, clicks and mobile interactions inside your site or app. The tracking data is then securely sent to Contentsquare servers, where it is aggregated and prepared for analysis. Contentsquare transforms this anonymous data into actionable insights and recommendations for your team.

- Impplementation of content sqaure pacxkage


###### Bloomreach Engagement
###### Facebook App Events


### Features & feature flags per region [TBC]

These are the features that we can turn on/ off on the fly for PROD or preProd(dev env) using remote config in Firebase including the EU region & language switching. 

**Firebase Remote Config** is a cloud service that lets you change the behavior and appearance of your app without requiring users to download an app update. When using Remote Config, you create in-app default values that control the behavior and appearance of your app.  
we can easily change the feature flag for Toolstation Mobile App Dev from Remote Config in Firebase.

###### Payments services used in differnet region ike NL: ideal, BrainTree/Paypal, G PAy, Apple Pay, Brain Tree Card

- Steps of App Development LifeCycle
### TS Deeplinks

The TS Deeplinks gives you access to a web browser link that directs you to a particular section of an already-installed app. Additionally, these links can be configured to direct viewers to particular content pages (such as events, news updates, and more) and transmit personalized data (like promo codes).

