# VTEX Checkout Events

Este archivo contiene una lista de eventos del checkout de VTEX que pueden ser manipulados, junto con una breve explicación de cada uno.

This file contains a list of VTEX checkout events that can be manipulated, along with a brief explanation of each.

En todos los casos, puedes utilizar tanto **arrow functions** como **closure functions** para manejar los eventos. La elección entre una y otra dependerá de tus preferencias personales y de las necesidades específicas de tu implementación, como el manejo del contexto de `this` y la claridad del código.

In all cases, you can use either **arrow functions** or **closure functions** to handle events. The choice between the two depends on your personal preference and the specific needs of your implementation, such as handling the `this` context and code readability.

```javascript
/**
 * Este evento se dispara cuando el orderForm se actualiza.
 * This event triggers when the orderForm is updated.
 */
$(window).on('orderFormUpdated.vtex', (event, orderForm) => console.log("orderFormUpdated.vtex"));

// closure functions example
$(window).on('orderFormUpdated.vtex', function(event, orderForm) {
    console.log("orderFormUpdated.vtex");
});

/**
 * Este evento se dispara cuando una solicitud de checkout termina.
 * This event triggers when a checkout request ends.
 */
$(window).on('checkoutRequestEnd.vtex', (event, orderForm) => console.log("checkoutRequestEnd.vtex"));

/**
 * Este evento se dispara durante el proceso de checkout.
 * This event triggers during the checkout process.
 */
$(window).on('checkout.vtex.com', (event, orderForm) => console.log("checkout.vtex.com"));

/**
 * Este evento se asocia con la interfaz de usuario de VTEX ID.
 * This event is associated with the VTEX ID user interface.
 */
$(window).on('.vtexIdUI', (event, orderForm) => console.log(".vtexIdUI"));

/**
 * Este evento se dispara cuando un usuario ha sido autenticado.
 * This event triggers when a user has been authenticated.
 */
$(window).on('authenticatedUser.vtexid', (event, orderForm) => console.log("authenticatedUser.vtexid"));

/**
 * Este evento se dispara cuando el proceso de autenticación de VTEX ID ha comenzado.
 * This event triggers when the VTEX ID authentication process has started.
 */
$(window).on('started.vtexid', (event, orderForm) => console.log("started.vtexid"));

/**
 * Este evento se dispara cuando la interfaz de VTEX ID ha sido renderizada.
 * This event triggers when the VTEX ID interface has been rendered.
 */
$(window).on('rendered.vtexid', (event, orderForm) => console.log("rendered.vtexid"));

/**
 * Este evento se dispara cuando se cierra la interfaz de VTEX ID.
 * This event triggers when the VTEX ID interface has been closed.
 */
$(window).on('closed.vtexid', (event, orderForm) => console.log("closed.vtexid"));

/**
 * Este evento se dispara cuando un usuario invitado (guest) inicia sesión.
 * This event triggers when a guest user logs in.
 */
$(window).on('guestUser.vtexid', (event, orderForm) => console.log("guestUser.vtexid"));

/**
 * Este evento se dispara cuando el token de VTEX ID ha sido refrescado.
 * This event triggers when the VTEX ID token has been refreshed.
 */
$(window).on('tokenRefreshed.vtexid', (event, orderForm) => console.log("tokenRefreshed.vtexid"));

/**
 * Este evento se dispara cuando se selecciona un idioma/localización.
 * This event triggers when a locale is selected.
 */
$(window).on('localeSelected.vtex', (event, orderForm) => console.log("localeSelected.vtex"));

/**
 * Este evento se dispara cuando un componente ha sido validado.
 * This event triggers when a component has been validated.
 */
$(window).on('componentValidated.vtex', (event, orderForm) => console.log("componentValidated.vtex"));

/**
 * Este evento se dispara durante el proceso de validación.
 * This event triggers during the validation process.
 */
$(window).on('validate.vtex', (event, orderForm) => console.log("validate.vtex"));

/**
 * Este evento se dispara cuando comienza la búsqueda de una dirección.
 * This event triggers when an address search starts.
 */
$(window).on('addressSearchStart.vtex', (event, orderForm) => console.log("addressSearchStart.vtex"));

/**
 * Este evento se dispara cuando se obtienen los resultados de la búsqueda de una dirección.
 * This event triggers when the address search results are returned.
 */
$(window).on('addressSearchResult.vtex', (event, orderForm) => console.log("addressSearchResult.vtex"));

/**
 * Este evento se dispara cuando se habilita un componente o funcionalidad.
 * This event triggers when a component or feature is enabled.
 */
$(window).on('enable.vtex', (event, orderForm) => console.log("enable.vtex"));

/**
 * Este evento se dispara cuando se deshabilita un componente o funcionalidad.
 * This event triggers when a component or feature is disabled.
 */
$(window).on('disable.vtex', (event, orderForm) => console.log("disable.vtex"));

/**
 * Este evento se dispara cuando comienza un proceso de carga.
 * This event triggers when a loading process starts.
 */
$(window).on('startLoading.vtex', (event, orderForm) => console.log("startLoading.vtex"));

/**
 * Este evento se dispara cuando la API de Google Maps ha sido cargada.
 * This event triggers when the Google Maps API has loaded.
 */
$(window).on('googleMapsAPILoaded.vtex', (event, orderForm) => console.log("googleMapsAPILoaded.vtex"));

/**
 * Este evento se dispara cuando las claves de la dirección han sido actualizadas.
 * This event triggers when the address keys have been updated.
 */
$(window).on('addressKeysUpdated.vtex', (event, orderForm) => console.log("addressKeysUpdated.vtex"));
```

