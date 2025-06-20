pipeline {
    agent any
    parameter {
        string(Name:'person', defaultValue:'subhash', decription:'my name is subhash')
        text(Name:'kairam', defaultVaule:'', decription:'text me subhashkairam')
        booleanParam(Name:'umasatya', defaultValue:'true', decription :'this is ture')
        choice(Name:'CHOOICE', defaultValue: ['one','two','three'] decription :'pick something')
        password(Name:'PASSWORD'defaultValue:'SECRETE',decription: 'enter password')
    }
    stages {
        stage('example') {
            steps {
            echo "Hello ${params.person}"
            echo "kairam:${perams.kairam}"
            echo "umasatya:${params.kairam}"
            echo "SELECTED Choice is :${params.CHOICE}"
            echo "Password entered is : ${params.PASSWORD}"
         }
      }
   }
}
