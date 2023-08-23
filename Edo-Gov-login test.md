## Cypress Login code
```cypess
  // describe('Login test', ()=>{
//     beforeEach( ()=>{
//      cy.visit('https://portal-test.greenzonetechnologies.com.ng/')
//     })

//     it('login with invalid email', ()=>{
//      cy.get('[name=email]').type('email')
//      cy.get('[name=password]').type('password')
//      cy.get('.m-b-10').click()
//     })


//        it('login with invalid password', ()=>{
//      cy.get('[name=email]').type('Email')
//      cy.get('[name=password]').type('password')
//      cy.get('.m-b-10').click()
//     })


//        it('login with valid details', ()=>{
//      cy.get('[name=email]').type('email')
//      cy.get('[name=password]').type('password')
//      cy.get('.m-b-10').click()

//      cy.contains('Human').click
//      cy.visit('https://training-test.greenzonetechnologies.com.ng/training-manager')

//     })

    //  it('change password', ()=>{
    //    cy.contains('Change password').click()
    //    cy.get('[placeholder=Email]').type('o.onwubolu@greenzonetechnologies.com.ng')
    //    cy.contains('Reset Password').click()
    //})

      // it('Human Resources', ()=>{
        
      // })
//})


describe('Login page', () => {
  it('Logs in successfully', () => {
    // Visit the login page
    cy.visit('https://portal-test.greenzonetechnologies.com.ng/');

    // Fill in the email and password fields
    cy.get('input[name=email]').type('email');
    cy.get('input[name=password]').type('password');

    // Click the login button
    cy.get('.m-b-10').click()

   
  });

  it('Shows error message with invalid credentials', () => {
    // Visit the login page
    cy.visit('https://portal-test.greenzonetechnologies.com.ng/');

    // Fill in invalid email and password fields
    cy.get('input[name=email]').type('invalid@example.com');
    cy.get('input[name=password]').type('invalidpassword');

    // Click the login button
    cy.get('.m-b-10').click()

    
  });
});
```
