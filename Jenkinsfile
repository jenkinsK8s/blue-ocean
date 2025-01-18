pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          environment {
            JOB_NAME = 'SONGPA'
          }
          steps {
            sh '''!#/bin/bash


echo "Jenkins Job Name: $JOB_NAME"'''
          }
        }

        stage('build2') {
          environment {
            JOB_NAME = 'GANGNAM'
          }
          steps {
            sh '''#!/bin/bash

echo "Jenkins Job Name: $JOB_NAME"'''
          }
        }

      }
    }

  }
}