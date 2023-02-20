# STORE THEME MATTELSA


<!-- DOCS-IGNORE:start -->
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->
<!-- DOCS-IGNORE:end -->

Clon de la pagina [Mattelsa](https://www.mattelsa.net/) con fines de aprendizaje y practica para emplear  **VTEX IO**  

![image](https://user-images.githubusercontent.com/83648336/220169119-54f7cffe-d344-4159-a0bd-44ee3e2f5259.png)


## Configuración

1. Instalar [VTEX IO CLI](https://developers.vtex.com/docs/guides/vtex-io-documentation-vtex-io-cli-install)
2. Guiarse de la siguiente documentación [Storefront](https://developers.vtex.com/docs/guides/getting-started-3) para [iniciar sesión](https://developers.vtex.com/docs/guides/vtex-io-documentation-1-basicsetup), de igual forma se encuentra información para crear un workspace, también se puede referir a la siguiente documentación [Creating a Development workspace](https://developers.vtex.com/docs/guides/vtex-io-documentation-creating-a-development-workspace)
   ```console
      vtex use <workspace>
   ```
3. Clonar el repositorio [store-theme](https://github.com/vtex-apps/store-theme)
4. Modificar el `manifest.json`
     ```json 
        {
          "vendor": "itgloberspartnercl",
          "name": "mattelsaclothe-store-theme",
          "version": "0.0.1",
        }
     ``` 
      **vendor:** nombre del cliente o información suministrada por él

      **name:** nombre del componente

      **version:** versión del componente

   Agregar en la sección `builders` dentro del `manifest.json` un `store`

    ```json   
        "store" : "0.x"
    ```
   
5. Instalar `vtex.store-sitemap` y `vtex.store`
    ```console  
        vtex install vtex.store-sitemap vtex.store -f
    ```
    
    Verificar la instalación con `vtex list`
    
6. Desinstalar el tema por defecto ejecutando el siguiente comando 
    ```console  
        vtex uninstall vtex.store-theme@0.0.1
    ```
7. Teniendo el `manifest.json` del template de la tienda, se realiza el paso de linkear la aplicación al espacio de trabajo, para eso ejecute el siguiente comando
    ```console  
        vtex link
    ```
    
    Posterior a la ejecución, en consola podra observar lo siguiente: 
    ![image](https://user-images.githubusercontent.com/83648336/220174728-df80fa49-3f1e-49d6-9c50-4589efe73dd6.png)

    Donde podrá encontrar el link de acceso a su pagina. También puede ejecutar el siguiente comando para abrir una ventana del navegador con el preview de la tienda
    ```console  
        vtex browse
    ```

## Dependencies

- store-theme

## Store Components Apps
    ```json
     "dependencies": {
        "vtex.store": "2.x",
        "vtex.store-header": "2.x",
        "vtex.product-summary": "2.x",
        "vtex.store-footer": "2.x",
        "vtex.store-components": "3.x",
        "vtex.styleguide": "9.x",
        "vtex.slider": "0.x",
        "vtex.carousel": "2.x",
        "vtex.shelf": "1.x",
        "vtex.menu": "2.x",
        "vtex.minicart": "2.x",
        "vtex.product-details": "1.x",
        "vtex.product-kit": "1.x",
        "vtex.search-result": "3.x",
        "vtex.search": "2.x",
        "vtex.login": "2.x",
        "vtex.my-account": "1.x",
        "vtex.flex-layout": "0.x",
        "vtex.rich-text": "0.x",
        "vtex.store-drawer": "0.x",
        "vtex.locale-switcher": "0.x",
        "vtex.product-quantity": "1.x",
        "vtex.product-identifier": "0.x",
        "vtex.product-specification-badges": "0.x",
        "vtex.product-review-interfaces": "1.x",
        "vtex.telemarketing": "2.x",
        "vtex.order-placed": "2.x",
        "vtex.stack-layout": "0.x",
        "vtex.tab-layout": "0.x",
        "vtex.responsive-layout": "0.x",
        "vtex.slider-layout": "0.x",
        "vtex.iframe": "0.x",
        "vtex.breadcrumb": "1.x",
        "vtex.sticky-layout": "0.x",
        "vtex.add-to-cart-button": "0.x",
        "vtex.store-image": "0.x",
        "vtex.store-link": "0.x",
        "vtex.store-icons": "0.x",
        "vtex.overlay-layout": "0.x",
        "vtex.modal-layout": "0.x",
        "vtex.product-list": "0.x",
        "vtex.product-price": "1.x",
        "vtex.disclosure-layout": "1.x",
        "vtex.store-newsletter": "1.x",
        "vtex.checkout-summary": "0.x",
        "vtex.category-menu": "2.x",
        "vtex.css-handles": "0.x",
      }
    ```

## Peer Dependencies

    ```json
       "peerDependencies": {
           "vtex.questions-and-answers": "0.x",
           "vtex.mega-menu": "2.x"
        }
    ```


### Custom Apps

1. Botón WhatsApp
2. Bullets diagramation
3. Custom Department Search
4. Add to cart info
5. PDF Reader
6. Quick order
7. Custom Grid

    ```json
        "itgloberspartnercl.whatsapp-button": "0.x",
        "itgloberspartnercl.bullets-diagramation": "0.x",
        "itgloberspartnercl.add-to-cart-info": "0.x",
        "itgloberspartnercl.custom-department-search": "0.x",
        "itgloberspartnercl.pdf-reader": "0.x",
        "itgloberspartnercl.quick-order": "0.x",
        "itgloberspartnercl.special-diagramation": "0.x"
    ```


<!-- DOCS-IGNORE:start -->

## Colaboradores ✨

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

Mariana Orrego Franco

<!-- DOCS-IGNORE:end -->
