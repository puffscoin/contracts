#escrow.sol

escrow.sol is deployed to the PUFFScoin mainnet at 0xbC0C17752743cbc45D295742c97FAa7cD44EDA16

compiler: Remix
version: 0.4.20+commit.3155dd80

METADATAHASH
"a22056dbdb99dddebdfd9f68152ad8cd2a13b557cb2dbd757a4e52ef58aaa311"

SWARMLOCATION
"bzzr://a22056dbdb99dddebdfd9f68152ad8cd2a13b557cb2dbd757a4e52ef58aaa311"

CONTRACT ABI:
[
	{
		"constant": false,
		"inputs": [
			{
				"name": "_id",
				"type": "uint256"
			}
		],
		"name": "participantPut",
		"outputs": [],
		"payable": true,
		"stateMutability": "payable",
		"type": "function"
	},
	{
		"constant": false,
		"inputs": [
			{
				"name": "_id",
				"type": "uint256"
			}
		],
		"name": "participantCancel",
		"outputs": [],
		"payable": false,
		"stateMutability": "nonpayable",
		"type": "function"
	},
	{
		"constant": false,
		"inputs": [
			{
				"name": "_id",
				"type": "uint256"
			}
		],
		"name": "participantPayout",
		"outputs": [
			{
				"name": "",
				"type": "bool"
			}
		],
		"payable": false,
		"stateMutability": "nonpayable",
		"type": "function"
	},
	{
		"constant": false,
		"inputs": [
			{
				"name": "_id",
				"type": "uint256"
			}
		],
		"name": "participantRelease",
		"outputs": [],
		"payable": false,
		"stateMutability": "nonpayable",
		"type": "function"
	},
	{
		"constant": false,
		"inputs": [
			{
				"name": "_name",
				"type": "bytes8"
			}
		],
		"name": "createEscrow",
		"outputs": [],
		"payable": false,
		"stateMutability": "nonpayable",
		"type": "function"
	},
	{
		"constant": true,
		"inputs": [],
		"name": "seq",
		"outputs": [
			{
				"name": "",
				"type": "uint256"
			}
		],
		"payable": false,
		"stateMutability": "view",
		"type": "function"
	},
	{
		"constant": false,
		"inputs": [
			{
				"name": "_seq",
				"type": "uint256"
			},
			{
				"name": "_amount",
				"type": "uint80"
			},
			{
				"name": "_who",
				"type": "address"
			},
			{
				"name": "_beneficiary",
				"type": "address"
			}
		],
		"name": "addParticipant",
		"outputs": [],
		"payable": false,
		"stateMutability": "nonpayable",
		"type": "function"
	},
	{
		"anonymous": false,
		"inputs": [
			{
				"indexed": false,
				"name": "seq",
				"type": "uint256"
			},
			{
				"indexed": false,
				"name": "_name",
				"type": "bytes8"
			}
		],
		"name": "Created",
		"type": "event"
	},
	{
		"anonymous": false,
		"inputs": [
			{
				"indexed": false,
				"name": "seq",
				"type": "uint256"
			},
			{
				"indexed": false,
				"name": "participant",
				"type": "address"
			}
		],
		"name": "ParticipantPaid",
		"type": "event"
	},
	{
		"anonymous": false,
		"inputs": [
			{
				"indexed": false,
				"name": "seq",
				"type": "uint256"
			},
			{
				"indexed": false,
				"name": "participant",
				"type": "address"
			}
		],
		"name": "ParticipantReleased",
		"type": "event"
	},
	{
		"anonymous": false,
		"inputs": [
			{
				"indexed": false,
				"name": "seq",
				"type": "uint256"
			},
			{
				"indexed": false,
				"name": "participant",
				"type": "address"
			}
		],
		"name": "ParticipantCancelled",
		"type": "event"
	},
	{
		"anonymous": false,
		"inputs": [
			{
				"indexed": false,
				"name": "seq",
				"type": "uint256"
			}
		],
		"name": "Finished",
		"type": "event"
	}
]



