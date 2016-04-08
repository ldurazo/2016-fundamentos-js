# Prototype Chain

Cuando se quiere usar una variable de un objeto el orden en que se busca es el siguiente:

* El contexto (`this`) del objeto

* El `prototype` del objecto

* El `prototype` del `prototype`

* El `prototype` del `prototype` del `prototype`

* El `prototype` del `prototype` del `prototype` del `prototype`

* Hasta que el `prototype` sea `null`

---