> este es un diccionario provisional a modo de guia y esta construido a partir de las columnas que quedaron del preprocesamiento de los datos.

- **factu_nume**: Número de facturacion, identificacion de la venta

- **linea_nume**:  identificador del dispositivo con el que se registro la venta

- **produc**: codigo de identificacion del producto

- **canti**: cantidad de productos vendidos 

- **precio_uni**: precio por unidad 

- **boni_porcen**: porcentaje bonificado 

- **boni_impor**  importe bonificado. Esta relacionado con el precio unitario,  los valores bonificados correspondan a articulos en promos.

- **iva1_impor**: iva sobre el importe.

- **descrip**: descripcion del articulo vendido (nombre del producto, catacteristicas como peso, unidades etc)

- **impor_grav**: (*desconocido*)

- **secuen**: (*desconocido*) aunque la relacion con **linea_nume** es 1:1 por lo que parece ser una columna redundante

- **uni_medi**: meida de unidad de venta
    - UN: unidad
    - DI: caja 
    - BU: peso 

- **conver**: (*desconocido*) parece tener una fuerte correlacion con **canti** aunque no en todos los casos es 1:1

- **linea_nume_auxi**: (*desconocido*) aunque la relacion con **linea_nume** es 1:1 por lo que parece ser una columna redundante

- **canti_venta**: (*desconocido*) esta fuertemente relacionado con **canti** aunque la relacion rara vez es 1:1 y no hay info en particular sobre bonificaciones por si se tratase de los articulos vendidos son promociones

- **precio_uni_ori** : precio unitario original , la columna posee una correlacion 1:1 con la columna **precio_uni** por lo que parece ser una columna redundante

- **iva1_impor_ori**: iva sobre **impor_ori**, los valores poseen una correlacion 1:1 con la columna **iva1_impor** por lo que parecer ser una columna redundante

- **impor_grava_ori**: (*desconocido*) tiene una relacion 1:1 don **impor_grava** por lo que parece ser una columna redundante

- **boni_porcen_precio**: (*desconocido*) no hay relacion clara con **boni_porcen**

- **boni_impor_precio**: (*desconocido*) no hay relacion clara con **boni_impor**

- **boni_impor_ori_precio**: (*desconocido*) no posee realcion con **boni_impor_ori** pero si tiene una relacion 1:1 con **boni_impor_ori_precio** por lo que parece ser una columna redundante

- **agru_linea_nume**: (*desconocido*) posee una correlacion lineal con la columna **linea_nume** aunque no siempre se respeta, los valores, cuando son distintos de 0, parecen ser {linea_nume} - 1, aunque no siembpre es asi.

- **precio_uni_neto**: valor unitario neto de los productos.

- **precio_total**: precio total de venta.

- **sucur**:  sucursal, codificado en 3 categorias;
    - 1
    - 9
    - 12

- **fecha**: fecha de realizacion de la venta, formato {dia}/{mes}/{año} {hora}:{min}:{seg}

- **cliente**: codigo de cliente, cada cliente posee una clasificacion

- **total**: precio de venta total,  no tiene correlacion directa con **precio_total**

- **iva1**: iva sobre **total**

- **lista_precios**:  clasificacion en 14 categorias distintas, posiblemente numero de catalogo 
    - 3
    - 48
    - 13
    - 4
    - 53
    - 0
    - 54
    - 15
    - 22
    - 11
    - 21
    - 2
    - 60
    - 16

- **usua**:  clasificacion de usuario en 4 categorias numericas, posiblemente clasificacion del vendedor 
    - 24
    - 34
    - 58
    - 1

- **pedi_nume**:  codigo numerico del pedido 

- **pedi_sucur**:  clasificacion numerica de la sucursal sobre la que se realizo el pedido 
    - 1
    - 9
    - 12

- **impor_gravado**: (*desconocido*)

- **entre_lugar**:  clasificacion numerica del lugar de entrega, tieen caracter binario.
    - 1
    - 2

- **entre_fecha**: fecha de entrega, formato {dia}/{mes}/{año} {hora}:{min}:{seg}

- **fecha_regis**: fecha de registro, formato {dia}/{mes}/{año} {hora}:{min}:{seg}. La fecha de registro es habitualmente un dia antes que la fecha de entrega o el mismo dia

- **conver_alter**: (*desconocido*)

- **impre_marca**: (*desconocido*) clasificacion numerica en 6 categorias
    - 1
    - 2
    - 3
    - 4
    - 5
    - 6

- **fecha_alta**: fecha de alta, formato {dia}/{mes}/{año} {hora}:{min}:{seg}

- **nombre**: nombre del comprador (punto de venta)

- **cuit**: cuit del comprador (punto de venta), no todos los datos estan completos, hay cuits faltantes

- **orden_compra_nume**:numero del orden de compra

- **vende**:  clasificacion del tipo de vendedor ?
    - 1
    - 2

- **total_ori**:  total original, correlacionado 1:1 con **total** por lo que parece ser una columna redundante

- **iva1_ori**: iva sobre **total_ori**, correlacionado 1:1 con **iva1** por lo que parece ser una columna redundante

- **impor_gravado_ori**: (*desconocido*) correlacionado 1:1 con **impor_gravado** por lo que parece ser una columna redundante

- **tipo_negocio**: clasificacion numerica sobre el tipo de negocio
    - 1
    - 2

- **factu_codi**: codigo string de la factura, el codigo parece ser una codificacion del tiempo de la venta 
    - FCA9
    - FCB9
    - FEA
    - FEA1
    - FEA4
    - FEB
    - FEB1
    - FEB4

- **pedi_codi**: codigo string del tipo de pedido
    - PEDIE
    - PEDIM

- **factu_letra**: tipo de factura
    - B

- **iva_cate**: categoria del iva 
    - EX
    - MI
    - NC
    - RI
    - RM
    - RS
    - cf

- **host_name_alta**: (*desconocido*)
    - NBDC-029
    - NBDC-030
    - SERVER
    - SERVER01
    - SERVER03
    - SRVDC902

- **estado_talon**: (*desconocido*)
    - O
    - P
    - R
