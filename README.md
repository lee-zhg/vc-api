# Watson Video Recongnition on Cloud -  Node.js Sample Code for image classification

The code in this repository provides a simple implementation of an app running on Node.js runtime demonstrating how to connect Node.js applications to the Watson Video Recongnition.


## Run the app locally

1. If you do not already have a Bluemix account, [sign up here](https://console.ng.bluemix.net/registration/)

2. If you have not already, [download node.js](https://nodejs.org/en/download/) and install it on your local machine.

3. Clone the app to your local environment from your terminal using the following command:

  ```
    git clone https://github.com/lee-zhg/vc-api
  ```

4. `cd` into this newly created directory

5. Install the required npm and bower packages using the following command

  ```
  npm install
  ```

6. Replace 3 pieces of information

  * iam_apikey - the API key of Watson Image Recognition service instance
  * classifier_ids - classifier_id of your VC model
  * images_file - you also need to copy your testing image file to the same folder, and update the file name in the sample code

7. Run the sample code locally with the following command

  ```
  node app.js
  ```
8. You should see output similar to

  ```
  {
    "images": [
      {
        "classifiers": [
          {
            "classifier_id": "lijing_1744016643",
            "name": "lijing",
            "classes": [
              {
                "class": "Burned Home",
                "score": 0.905
              }
            ]
          }
        ],
        "image": "test04.jpg"
      }
    ],
    "images_processed": 1,
    "custom_classes": 2
  }
  ```

