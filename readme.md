- rodar projeto cypress - npx cypress open
- rodar backend - cd server (entrar na pasta server) e - npm start
- rodar frontend - cd web (entrar na pasta web) e - npm start

- Ctrl+; Comenta ou descomenta trechos de código
- Rodar teste em outro navegador (firefox): npx cypress run --browser firefox

- o should é bem poderoso e pode ser usado de várias formas:
    - cy.url().should('eq', 'http://localhost:3000/dashboard') - eq = equal (igual a)
    - cy.contains('Cadastrar especialista').should('be.visible').click() - be.visible = (deve estar visivel)
    - cy.get('[type="checkbox"]').should('have.attr', 'aria-label', 'Atende por plano?').and('not.be.checked') - have.attr = (tem o atributo) e o texto do aria-label no caso e .and complementa a operação .and('not.be.checked') - essa linha de comando pega o primeiro checkbox que ela encontrar na pagina que não esteja marcado (checado)
