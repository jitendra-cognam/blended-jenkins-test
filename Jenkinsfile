#!/usr/bin/env groovy

pipeline {
    agent any
    options {
        timestamps()
    }
    stages {
        stage('Build project A') {
            when {
                changeset "project1/**"
            }
            steps {
                build 'project1'
            }
        }
        stage('Build project B') {
            when {
                changeset "project2/**"
            }
            steps {
                build 'project2'
            }
        }
    }
}
