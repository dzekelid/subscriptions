swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SubscribeToDataset:
    get:
      summary: Subscribe To Dataset
      description: Subscribes to receive notifications when a dataset is modified
        by another device.
      operationId: subscribeToDataset
      x-api-path-slug: actionsubscribetodataset-get
      parameters:
      - in: query
        name: DatasetName
        description: The name of the dataset to subcribe to
        type: string
      - in: query
        name: DeviceId
        description: The unique ID generated for this device by Cognito
        type: string
      - in: query
        name: IdentityId
        description: Unique ID for this identity
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Dataset