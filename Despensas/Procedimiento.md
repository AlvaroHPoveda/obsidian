## Tarea: Causal Retoma

### Archivos a modificar

- **`enum.ts`**
  - En `causalesFabrica` → adicionar el código de la causal retoma

- **`fabrica-credito-gestiones.component.ts`**
  - En `ngOnInit` → `this.listaCausalesAgestionar` → agregar el código de la causal

- **Personas (recursos generales)**
  - Buscar `listaCausalesAgestionar` y agregar el código causal

- **`fabrica-credito-gestion-despensas.component.html`**
  - Agregar el botón y su funcionalidad en el `.ts`

---

### Consultas SQL

```sql
select * from listascausalessolicitudes l where Codigo = 'RECOTA'
```

```sql
select * from solicitudesestadoshistoricos s 
where IdSolicitud = '9A81CF53-9E7D-471E-BD34-647D718F6806' 
order by FechaCambioEstado desc
```

```sql
select * from plataformasdigitales p where IdPlataformaDigital = ''
```

---

### IDs importantes

| Nombre | Valor |
|--------|-------|
| IdLista | `55D176BB-81D3-4920-9D11-E05C3EE59EDD` |
| IdCausalSolicitud | pega id `RECOTA` en el primer registro |
| IdCausal | pega id `RECOTA` |

---

### Servicio

- **Nombre:** Plataformas Digitales
- Buscar donde se lanza el `IdPlataformaDigital`
- [Endpoint](https://analizamosdev.hexasolutions.co:8440/negocioautogestionado/api/plataformasDigitales/3F1833B9-B2E8-41B3-86C5-72645999651C)