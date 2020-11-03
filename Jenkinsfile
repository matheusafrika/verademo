pipeline {
  agent any
  stages {
    stage('Veracode scan') {
      steps {
        veracode(applicationName: 'Verademo - smiles', criticality: 'VeryHigh', debug: true, scanName: '$buildnumber', timeout: 60, uploadIncludesPattern: '**/**.jar, **/**.war', vid: '0638ee443eb6afad24ec5ede711b4fd2', vkey: '656db8a3a0c9f1a406295cd25e3c017beead2909a3aeb66d38a6bf56530a6de6e5597300e918f814c3cef586baa813a52d4e70054308f9bcff532e17f4f4b309', waitForScan: true)
      }
    }

  }
}