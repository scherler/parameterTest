node() {
   // adds job parameters within jenkinsfile
   properties([
     parameters([
       booleanParam(
         defaultValue: true,
         description: 'isFoo should be false',
         name: 'isFoo'
       ),
       booleanParam(
         defaultValue: false,
         description: 'isBar should be true',
         name: 'isBar'
       ),
     ])
   ])

   // test the false value
   print 'DEBUG: parameter isFoo = ' + params.isFoo
   print "DEBUG: parameter isFoo = ${params.isFoo}"
   sh "echo sh isFoo is ${params.isFoo}"
   if (params.isFoo) { print "THIS SHOULD DISPLAY" }

   // test the true value
   print 'DEBUG: parameter isBar = ' + params.isBar
   print "DEBUG: parameter isBar = ${params.isBar}"
   sh "echo sh isBar is ${params.isBar}"
   if (params.isBar) { print "this should NOT display" }
}
