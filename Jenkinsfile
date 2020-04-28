#!/usr/bin/env groovy

properties([
 parameters([
  choice( choices:['non-prod', 'prod'], name:"Environment"),
  string(name: "Loopvalue", value="5")
  ])
])

stages {
 stage("First") {
  def rang= 1..${params.Loopvalue}
  println "Numbers are ${rang}"
 }
}

