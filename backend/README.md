Getting up and running is as easy as 1, 2, 3.

1. Make sure you have [NodeJS](https://nodejs.org/) and [npm](https://www.npmjs.com/) installed.
2. Install your dependencies

    ```
    cd path/to/backend; npm install
    ```

3. Start your app

    ```
    npm start
    ```
	
API URLs

1) BOX 

	<API_URL>/box
	Method: POST
	
	1) to get box id
		body: {
			getBoxId: true,
			barcode: barcode
		}
	2) to get Box Status
		body: {
			getBoxStatus: true,
			barcode: barcode
		}

2) CLOCK

	<API_URL>/clock
	Method: POST

	1) to clock In
		body: {
			clockIn: true,
			boxId: boxId,
			userId: userId,
			comment: comment
		}

	2) to clock OUT
		body: {
			clockOut: true,
			boxId: boxId,
			userId: userId,
			state: state,
			comment: comment
		}

	3) TO GET CLOCK INFO
		body: {
			clockInfo: true,
			userId: userId
		}

3) PRODTASK

	<API_URL>/prodtask
	Method: POST
		body: {}

4) STATES

	<API_URL>/states
	Method: POST
		body: {}


4) LOGIN

	<API_URL>/login
	Method: POST
		body: {
			username: username,
			password: password
		}














