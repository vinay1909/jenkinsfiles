#!/usr/bin/env groovy

agent any 

properties([
 parameters([ 
  choice( choices:['non-prod', 'prod'], name:"Environment"),
  string( name: "Loopvalue", defaultValue="5"),
  ])
])

stages {
 stage("First") {
  def rang= 1..${params.Loopvalue}
  println "Numbers are ${rang}"
 }
}

