pipeline {
    agent any

    stages {
        # Download and Run Hyperexecute stage (optional)
        stage('Download & Run Hyperexecute') {
            steps {
                # Download Hyperexecute CLI for macOS (adjust for other OS)
                sh name: 'Download Hyperexecute CLI', script: 'wget https://downloads.lambdatest.com/hyperexecute/darwin/hyperexecute'
                # Grant execute permission to the downloaded binary
                sh name: 'Make Hyperexecute executable', script: 'chmod +x hyperexecute'
                # Run Hyperexecute with user credentials and configuration file
                sh name: 'Run Hyperexecute Tests', script: './hyperexecute --user <your_username> --key <your_access_key> --config <your_yaml_file_path>
            }
        }
    }
}
