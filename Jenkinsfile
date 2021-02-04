#!/usr/bin/env groovy

pipeline {
    agent any
    stages {
        stage('Build project1') {
            when {
                changeset "project1/**"
            }
            steps {
                build 'project1'
            }
        }
        stage('Build project2') {
            when {
                changeset "project2/**"
            }
            steps {
                build 'project2'
            }
        }
    }
}
