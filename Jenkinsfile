#!/usr/bin/env groovy

pipeline {
  agent any

parameters {
  choice( choices:['non-prod', 'prod'], name:"Environment")
  string( name: "Loopvalue", defaultValue="5"),
}

stages {
 stage("First") {
  steps {
  def rang= 1..${params.Loopvalue}
  println "Numbers are ${rang}"
  }
 }
}
}
