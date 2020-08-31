# Video-Analyzer-Rekognition
Analyze the video when uploaded in to s3 using rekognition, triggers sns events using lamba functions and insert the result data in dynamo db

When the video file is uploaded in to s3,gets the info about the video using 'rekognition' by 'start_label_detection' function.
Triggers the SNS event when video is uploaded in to S3 and start the lambda function , upload the collected informations in DynamoDB table

# Command to add video in to s3 bucket using pathlib "upload_files(profile, path_name, bucket_name)"
  ---> pipenv run python upload-file.py --profile=pythonAutomation  "~/Downloads/Pexels Videos 2670.mp4" video-analyze-nk-01
