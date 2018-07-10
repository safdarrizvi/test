pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                    //Install required packages
                    sh '''
                        apt-get update
                        apt-get install -y zip python3-pip
                    '''

                    //Install AWS CLI
                    sh 'pip3 install awscli --upgrade'

                    //Set the AWS credentials
                    //sh '''
                    //    aws configure set aws_access_key_id "AKIAJZPHBAFQ6SNZNX2A"
                    //    aws configure set aws_secret_access_key "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"
                    //    aws configure set default.region "eu-west-1"
                    //'''
					//sh '''
                	//	aws cloudformation create-stack                                                                                                                                         \
					//		--stack-name TestBucket                                                                                                                      			\
					//		--role-arn arn:aws:iam::689349191276:role/TestBucketRole                                                                                                        \
					//		--capabilities CAPABILITY_IAM CAPABILITY_NAMED_IAM																													\
					//		--template-body file://store.template
                    //    aws cloudformation wait stack-create-complete --stack-name TestBucket
					//'''
					}
             }
         }
     }