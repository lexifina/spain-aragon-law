# Aragon: law history in git

The law of the autonomous community of Aragon (Comunidad Autónoma de Aragón, Spain) as a git history: one file per article, one commit per norm that changed it, dated the day the change took effect, with the amending norm as the commit's author. `git blame` names the norm behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `es-ar/`. Spain's national law is in [lexifina/spain-law](https://github.com/lexifina/spain-law).

The text is in Spanish, exactly as the BOE's consolidated text prints it. Texts in co-official languages are not included.

Basado en datos de la Agencia Estatal Boletín Oficial del Estado (<https://www.boe.es>). Every text here is a consolidated text for information only (texto consolidado de carácter meramente informativo), not an official publication.

## What this repository holds

260 norms with 822 versions so far: the Estatuto de Autonomía first, then the laws, decree-laws and legislative decrees in force that the BOE consolidates, oldest first, added in parts of about 50. 26 of them are repealed norms the BOE consolidates: their whole history is kept, and their last commit removes the text on the day the repeal took effect, credited to the repealing norm. Regulations are not included (the BOE consolidates no autonomic decrees or orders).

| Folder | Norm | Versions | History | BOE last updated |
| --- | --- | ---: | --- | --- |
| `estatuto-de-autonomia/` | Ley Orgánica 5/2007, de 20 de abril, de reforma del Estatuto de Autonomía de Aragón. | 3 | as first published, then each change: 23 April 2007 to 28 December 2022 | 2026-10-02 |
| `ley-1983-001/` | Ley 1/1983, de 28 de septiembre, por la que se determina la sede de las Cortes de Aragón. | 1 | as first published: 8 October 1983 | 2025-12-16 |
| `ley-1984-001/` | Ley 1/1984, de 16 de abril, por la que se declara "Día de Aragón" el 23 de abril, tradicional conmemoración de San Jorge. | 1 | as first published: 18 April 1984 | 2026-05-27 |
| `ley-1984-002/` | Ley 2/1984, de 16 de abril, sobre uso de la Bandera y el Escudo de Aragón. | 1 | as first published: 8 May 1984 | 2025-12-16 |
| `ley-1984-007/` | Ley 7/1984, de 27 de diciembre, reguladora de la iniciativa legislativa popular ante las Cortes de Aragón. | 2 | as first published, then each change: 24 January 1985 to 9 October 2014 | 2025-12-16 |
| `ley-1985-004/` | Ley 4/1985, de 27 de junio, Reguladora del Justicia de Aragón. | 6 | as first published, then each change: 3 July 1985 to 6 November 2025 | 2025-12-16 |
| `ley-1986-005/` | Ley 5/1986, de 17 de noviembre, de Salud Escolar. | 1 | as first published: 21 December 1986 | 2025-12-17 |
| `ley-1986-006/` | Ley 6/1986, de 28 de noviembre, de Archivos de Aragón. | 5 | as first published, then each change: 21 December 1986 to 19 June 2024 | 2025-12-17 |
| `ley-1986-007/` | Ley 7/1986, de 5 de diciembre, de Museos de Aragón. | 1 | as first published: 29 December 1986 | 2025-12-17 |
| `ley-1987-002/` | Ley 2/1987, de 16 de febrero, Electoral de la Comunidad Autónoma de Aragón. | 8 | as first published, then each change: 19 February 1987 to 28 February 2023 | 2026-02-24 |
| `ley-1987-008/` | Ley 8/1987, de 15 de abril, de creación, organización y control parlamentario de la Corporación Aragonesa de Radio y Televisión. | 9 | as first published, then each change: 12 May 1987 to 4 November 2023 | 2025-12-17 |
| `ley-1989-001/` | Ley 1/1989, de 24 de febrero, de Artesanía de Aragón. | 1 | as first published: 23 March 1989 | 2025-12-17 |
| `ley-1989-003/` | Ley 3/1989, de 21 de abril del Himno de Aragón. | 1 | as first published: 5 May 1989 | 2025-12-17 |
| `ley-1990-003/` | Ley 3/1990, de 4 de abril, del Consejo Aragonés de la Tercera Edad. | 3 | as first published, then each change: 17 April 1990 to 1 January 2005 | 2025-12-17 |
| `ley-1990-009/` | Ley 9/1990, de 9 de noviembre, del Consejo Económico y Social de Aragón. | 3 | as first published, then each change: 14 November 1990 to 21 December 2022 | 2025-12-17 |
| `ley-1991-001/` | Ley 1/1991, de 4 de enero, reguladora de las Cajas de Ahorros en Aragón. | 9 | as first published, then each change: 19 January 1991 to 16 July 2014 | 2025-12-17 |
| `decreto-legislativo-1991-001/` | Decreto Legislativo 1/1991, de 19 de febrero de la Diputación General de Aragón, por el que se aprueba el texto refundido de la Ley de Ordenación de la Función Pública de la Comunidad Autónoma de Aragón. | 20 | oldest version available, then each change: 2 March 1991 to 1 January 2024 | 2024-01-18 |
| `ley-1992-001/` | Ley 1/1992, de 17 de febrero, de medidas para la ordenación integral del Somontano del Moncayo. | 1 | as first published: 28 February 1992 | 2025-12-17 |
| `ley-1992-010/` | Ley 10/1992, de 4 de noviembre, de fianzas de arrendamientos y otros contratos. | 7 | as first published, then each change: 10 December 1992 to 4 February 2016 | 2025-12-17 |
| `ley-1993-002/` | Ley 2/1993, de 19 de febrero, por la que se crea el Instituto Aragonés de la Mujer. | 5 | as first published, then each change: 2 March 1993 to 30 July 2018 | 2025-12-17 |
| `ley-1994-009/` | Ley 9/1994, de 7 de octubre, reguladora de los Planes de Desarrollo Regional de los Fondos Estructurales de la Unión Europea. | 1 | as first published: 24 October 1994 | 2025-12-17 |
| `ley-1996-002/` | Ley 2/1996, de 14 de mayo, de Cámaras Agrarias de Aragón. | 2 | as first published, then each change: 23 May 1996 to 3 May 2001 | 2025-12-18 |
| `ley-1996-004/` | Ley 4/1996, de 22 de mayo, relativa al Instituto Aragonés de Servicios Sociales. | 4 | as first published, then each change: 28 May 1996 to 1 January 2021 | 2025-12-18 |
| `ley-1997-005/` | Ley 5/1997, de 3 de julio, de Creación del Colegio Profesional de Fisioterapeutas de Aragón. | 1 | as first published: 15 July 1997 | 2025-12-18 |
| `ley-1997-006/` | Ley 6/1997, de 3 de julio, de Creación del Colegio Profesional de Podólogos de Aragón. | 1 | as first published: 15 July 1997 | 2025-12-18 |
| `ley-1997-010/` | Ley 10/1997, de 17 de noviembre, por la que se instrumenta la aplicación del Plan Estratégico del Bajo Ebro Aragonés y se aprueban medidas para su mejor ejecución. | 1 | as first published: 25 November 1997 | 2025-12-18 |
| `ley-1997-011/` | Ley 11/1997, de 26 de noviembre, sobre Medidas Urgentes en Materia de Personal. | 5 | as first published, then each change: 6 December 1997 to 1 January 2001 | 2025-12-18 |
| `ley-1997-012/` | Ley 12/1997, de 3 de diciembre, de Parques Culturales de Aragón. | 1 | as first published: 1 January 1998 | 2025-12-18 |
| `ley-1998-001/` | Ley 1/1998, de 16 de febrero, sobre reclamaciones tributarias en la Comunidad Autónoma de Aragón. | 4 | as first published, then each change: 19 March 1998 to 1 January 2015 | 2025-12-18 |
| `ley-1998-002/` | Ley 2/1998, de 12 de marzo, de Colegios Profesionales de Aragón. | 3 | as first published, then each change: 9 April 1998 to 6 May 2010 | 2025-12-18 |
| `ley-1998-004/` | Ley 4/1998, de 8 de abril, de Medidas Fiscales, Financieras, de Patrimonio y Administrativas. | 15 | as first published, then each change: 13 April 1998 to 9 March 2018 | 2025-12-18 |
| `ley-1998-005/` | Ley 5/1998, de 14 de mayo, de los Consejos Escolares de Aragón. | 3 | as first published, then each change: 23 May 1998 to 4 February 2016 | 2025-12-18 |
| `ley-1998-007/` | Ley 7/1998, de 16 de julio, por la que se aprueban las Directrices Generales de Ordenación Territorial para Aragón. | 4 | as first published, then each change: 30 July 1998 to 10 March 2004 | 2025-12-18 |
| `ley-1998-008/` | Ley 8/1998, de 17 de diciembre, de Carreteras de Aragón. | 2 | as first published, then each change: 19 January 1999 to 1 January 2015 | 2025-12-18 |
| `ley-1998-014/` | Ley 14/1998, de 30 de diciembre, de los Transportes Urbanos de la Comunidad Autónoma de Aragón. | 5 | as first published, then each change: 28 January 1999 to 17 July 2023 | 2025-12-18 |
| `ley-1999-002/` | Ley 2/1999, de 24 de febrero, de Pesca en Aragón. | 2 | as first published, then each change: 24 March 1999 to 1 January 2015 | 2025-12-18 |
| `ley-1999-003/` | Ley 3/1999, de 10 de marzo, del Patrimonio Cultural Aragonés. | 12 | as first published, then each change: 30 March 1999 to 19 June 2024 | 2025-12-18 |
| `ley-1999-004/` | Ley 4/1999, de 25 de marzo, de Ordenación Farmacéutica para Aragón. | 5 | as first published, then each change: 7 April 1999 to 1 January 2015 | 2025-12-18 |
| `ley-1999-007/` | Ley 7/1999, de 9 de abril, de Administración Local de Aragón. | 17 | as first published, then each change: 17 July 1999 to 1 January 2023 | 2025-12-18 |
| `ley-1999-009/` | Ley 9/1999, de 9 de abril, de creación del Instituto Aragonés de Empleo. | 2 | as first published, then each change: 18 April 1999 to 26 June 2010 | 2025-12-18 |
| `ley-2000-002/` | Ley 2/2000, de 28 de junio, del Juego de la Comunidad Autónoma de Aragón. | 11 | oldest version available, then each change: 8 July 2000 to 11 April 2023 | 2025-12-18 |
| `decreto-legislativo-2000-004/` | Decreto Legislativo 4/2000, de 29 junio, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley del Instituto Aragonés de Fomento. | 4 | oldest version available, then each change: 30 June 2000 to 1 October 2019 | 2023-12-26 |
| `decreto-legislativo-2000-005/` | Decreto Legislativo 5/2000, de 29 junio, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley Reguladora del Instituto Tecnológico de Aragón. | 2 | oldest version available, then each change: 30 June 2000 to 1 January 2004 | 2023-12-26 |
| `ley-2000-005/` | Ley 5/2000, de 28 de noviembre, de Relaciones con las Comunidades Aragonesas del Exterior. | 1 | as first published: 2 January 2001 | 2025-12-18 |
| `ley-2000-006/` | Ley 6/2000, de 28 de noviembre, de Creación del Colegio Profesional de Protésicos Dentales de Aragón. | 1 | as first published: 2 January 2001 | 2025-12-18 |
| `ley-2000-007/` | Ley 7/2000, de 28 de noviembre, de Creación, por segregación, del Colegio Oficial de Licenciados en Educación Física y en Ciencias de la Actividad Física y del Deporte de Aragón. | 1 | as first published: 2 January 2001 | 2025-12-18 |
| `ley-2000-008/` | Ley 8/2000, de 28 de noviembre, de creación, por segregación, del Colegio Profesional de Doctores y Licenciados en Ciencias Políticas y Sociología de Aragón. | 1 | as first published: 2 January 2001 | 2025-12-18 |
| `ley-2000-009/` | Ley 9/2000, de 27 de diciembre, de creación de la Comarca del Aranda. | 1 | as first published: 31 December 2000 | 2025-12-18 |
| `ley-2000-010/` | Ley 10/2000, de 27 de diciembre, relativa a la Cooperación para el Desarrollo. | 1 | as first published: 31 December 2000 | 2025-12-18 |
| `ley-2001-003/` | Ley 3/2001, de 4 de abril, de prevención, asistencia y reinserción social en materia de drogodependencias. | 3 | as first published, then each change: 1 May 2001 to 16 July 2014 | 2025-12-18 |
| `ley-2001-007/` | Ley 7/2001, de 31 de mayo, de creación de la entidad pública Aragonesa de Servicios Telemáticos. | 3 | as first published, then each change: 28 June 2001 to 4 February 2016 | 2025-12-18 |
| `ley-2001-009/` | Ley 9/2001, de 18 de junio, de Creación de la Comarca de la Comunidad de Calatayud. | 1 | as first published: 16 August 2001 | 2025-12-18 |
| `ley-2001-011/` | Ley 11/2001, de 18 de junio, de Creación del Colegio Profesional de Terapeutas Ocupacionales de Aragón. | 1 | as first published: 28 June 2001 | 2025-12-18 |
| `ley-2001-012/` | Ley 12/2001, de 2 de julio, de la Infancia y la Adolescencia en Aragón. | 2 | as first published, then each change: 9 August 2001 to 17 June 2016 | 2025-12-18 |
| `ley-2001-013/` | Ley 13/2001, de 2 de julio, de Creación de la Comarca del Alto Gállego. | 1 | as first published: 27 August 2001 | 2025-12-18 |
| `ley-2001-014/` | Ley 14/2001, de 2 de julio, de Creación de la Comarca de Tarazona y el Moncayo. | 1 | as first published: 30 August 2001 | 2025-12-18 |
| `ley-2001-015/` | Ley 15/2001, de 3 de octubre, de creación, por segregación, del Colegio Profesional de Decoradores de Aragón. | 1 | as first published: 4 November 2001 | 2025-12-18 |
| `ley-2001-016/` | Ley 16/2001, de 29 de octubre, de Creación de la Comarca de Valdejalón. | 1 | as first published: 6 November 2001 | 2025-12-18 |
| `ley-2001-017/` | Ley 17/2001, de 29 de octubre, sobre la Plataforma Logística de Zaragoza. | 4 | as first published, then each change: 6 November 2001 to 27 August 2022 | 2025-12-18 |
| `ley-2001-018/` | Ley 18/2001, de 19 de noviembre, de creación de la Comarca de Campo de Borja. | 1 | as first published: 24 November 2001 | 2025-12-18 |
| `ley-2001-019/` | Ley 19/2001, de 4 de diciembre, del Instituto Aragonés de la Juventud. | 5 | as first published, then each change: 11 December 2001 to 7 May 2023 | 2025-12-18 |
| `ley-2001-021/` | Ley 21/2001, de 21 de diciembre, de Creación de la Comarca de la Ribera Alta del Ebro. | 1 | as first published: 27 December 2001 | 2025-12-18 |
| `ley-2001-022/` | Ley 22/2001, de 21 de diciembre, de Creación de la Comarca Gúdar-Javalambre. | 1 | as first published: 27 December 2001 | 2025-12-18 |
| `ley-2002-001/` | Ley 1/2002, de 13 de febrero, de Creación del Colegio Profesional de Diplomados en Trabajo Social y Asistentes Sociales de Aragón. | 1 | as first published: 21 March 2002 | 2025-12-18 |
| `ley-2002-002/` | Ley 2/2002, de 13 de febrero, de Creación del Colegio Profesional de Logopedas de Aragón. | 1 | as first published: 21 March 2002 | 2025-12-18 |
| `ley-2002-003/` | Ley 3/2002, de 25 de marzo, de creación de la Comarca del Cinca Medio. | 1 | oldest version available: 4 April 2002 | 2025-12-18 |
| `ley-2002-004/` | Ley 4/2002, de 25 de marzo, de creación de la Comarca de Somontano de Barbastro. | 1 | oldest version available: 4 April 2002 | 2025-12-18 |
| `ley-2002-006/` | Ley 6/2002, de 15 de abril, de Salud de Aragón. | 11 | as first published, then each change: 20 April 2002 to 2 October 2021 | 2025-12-18 |
| `ley-2002-007/` | Ley 7/2002, de 15 de abril, de creación de la Comarca del Matarraña/Matarranya. | 1 | as first published: 20 April 2002 | 2025-12-18 |
| `ley-2002-008/` | Ley 8/2002, de 3 de mayo, de Creación de la Comarca del Maestrazgo. | 1 | as first published: 9 May 2002 | 2025-12-18 |
| `ley-2002-009/` | Ley 9/2002, de 3 de mayo, de Creación de la Comarca de La Jacetania. | 1 | as first published: 9 May 2002 | 2025-12-18 |
| `ley-2002-010/` | Ley 10/2002, de 3 de mayo, de Creación de la Comarca del Bajo Aragón | 1 | as first published: 9 May 2002 | 2025-12-18 |
| `ley-2002-011/` | Ley 11/2002, de 14 de mayo, de Creación de la Comarca de Andorra-Sierra de Arcos. | 1 | as first published: 18 May 2002 | 2025-12-18 |
| `ley-2002-012/` | Ley 12/2002, de 28 de mayo, de creación de la Comarca de La Ribagorza. | 2 | as first published, then each change: 1 June 2002 to 1 March 2023 | 2025-12-18 |
| `ley-2002-013/` | Ley 13/2002, de 10 de junio, de creación de la Comarca de la Ribera Baja del Ebro. | 1 | as first published: 18 June 2002 | 2025-12-18 |
| `ley-2002-014/` | Ley 14/2002, de 10 de junio, de creación del Colegio Profesional de Delineantes de Huesca. | 1 | as first published: 18 June 2002 | 2025-12-18 |
| `ley-2002-015/` | Ley 15/2002, de 27 de junio, por la que se deja libre de ordenación el aprovechamiento de los pastos en la Comunidad Autónoma de Aragón. | 1 | as first published: 28 July 2002 | 2025-12-18 |
| `ley-2002-017/` | Ley 17/2002, de 5 de julio, de Creación de la Comarca de los Monegros. | 1 | as first published: 1 September 2002 | 2025-12-18 |
| `ley-2002-018/` | Ley 18/2002, de 5 de julio, de Creación de la Comarca de Campo de Daroca. | 1 | as first published: 1 September 2002 | 2025-12-18 |
| `ley-2002-019/` | Ley 19/2002, de 18 de septiembre, de creación, por segregación, del Colegio Profesional de Psicólogos de Aragón. | 1 | as first published: 26 September 2002 | 2025-12-18 |
| `ley-2002-020/` | Ley 20/2002, de 7 de octubre, de creación de la Comarca del Bajo Cinca/Baix Cinca. | 1 | as first published: 8 October 2002 | 2025-12-18 |
| `ley-2002-024/` | Ley 24/2002, de 12 de noviembre, de Creación de la Comarca de Campo de Belchite. | 1 | as first published: 16 November 2002 | 2025-12-18 |
| `ley-2002-025/` | Ley 25/2002, de 12 de noviembre, de Creación de la Comarca de la Litera/La Llitera. | 1 | as first published: 16 November 2002 | 2025-12-18 |
| `ley-2002-026/` | Ley 26/2002, de 26 de noviembre, de Creación de la Comarca de Cinco Villas. | 1 | as first published: 30 November 2002 | 2025-12-18 |
| `ley-2002-027/` | Ley 27/2002, de 26 de noviembre, de creación de la Comarca de Hoya de Huesca/Plana de Uesca. | 1 | oldest version available: 30 November 2002 | 2025-12-18 |
| `ley-2002-028/` | Ley 28/2002, de 17 de diciembre, de Creación de la Comarca de Cuencas Mineras. | 1 | as first published: 28 December 2002 | 2025-12-18 |
| `ley-2002-029/` | Ley 29/2002, de 17 de diciembre, de Creación del Centro de Investigación y Tecnología Agroalimentaria de Aragón. | 5 | as first published, then each change: 1 January 2003 to 4 February 2016 | 2025-12-18 |
| `ley-2002-031/` | Ley 31/2002, de 27 de diciembre, de Creación de la Comarca de Campo de Cariñena. | 1 | as first published: 9 January 2003 | 2025-12-18 |
| `ley-2003-001/` | Ley 1/2003, de 11 de febrero, de creación de la Comarca de la Sierra de Albarracín. | 1 | as first published: 22 February 2003 | 2025-12-18 |
| `ley-2003-005/` | Ley 5/2003, de 26 de febrero, de creación de la Comarca de Sobrarbe. | 1 | as first published: 8 March 2003 | 2025-12-18 |
| `ley-2003-007/` | Ley 7/2003, de 12 de marzo, de creación de la Comarca de la Comunidad de Teruel. | 1 | as first published: 3 April 2003 | 2025-12-18 |
| `ley-2003-008/` | Ley 8/2003, de 12 de marzo, de Creación de la Comarca del Bajo Martín. | 1 | as first published: 20 March 2003 | 2025-12-18 |
| `ley-2003-011/` | Ley 11/2003, de 19 de marzo, de Protección Animal en la Comunidad Autónoma de Aragón. | 4 | as first published, then each change: 26 June 2003 to 17 July 2023 | 2025-12-18 |
| `ley-2003-012/` | Ley 12/2003, de 24 de marzo, de Creación de la Comarca de Bajo Aragón-Caspe/Baix Aragó-Casp. | 1 | as first published: 27 March 2003 | 2025-12-18 |
| `ley-2003-013/` | Ley 13/2003, de 24 de marzo, de Creación de la Comarca del Jiloca. | 1 | as first published: 27 March 2003 | 2025-12-18 |
| `ley-2003-016/` | Ley 16/2003, de 24 de marzo, sobre publicidad institucional. | 3 | as first published, then each change: 1 May 2003 to 20 March 2012 | 2026-07-13 |
| `ley-2003-017/` | Ley 17/2003, de 24 de marzo, por la que se regula la organización de las enseñanzas artísticas superiores en Aragón. | 2 | as first published, then each change: 12 April 2003 to 1 January 2013 | 2025-12-18 |
| `ley-2003-018/` | Ley 18/2003, de 11 de julio, sobre designación de Senadores en representación de la Comunidad Autónoma de Aragón. | 1 | as first published: 12 July 2003 | 2025-12-18 |
| `ley-2003-024/` | Ley 24/2003, de 26 de diciembre, de medidas urgentes de política de vivienda protegida. | 18 | as first published, then each change: 1 January 2004 to 1 January 2023 | 2025-12-18 |
| `decreto-legislativo-2004-001/` | Decreto Legislativo 1/2004, de 27 de julio, del Gobierno de Aragón, por el que se aprueba el Texto Refundido de las Tasas de la Comunidad Autónoma de Aragón. | 18 | oldest version available, then each change: 10 August 2004 to 23 October 2021 | 2025-04-29 |
| `ley-2004-008/` | Ley 8/2004, de 20 de diciembre, de Medidas Urgentes en Materia de Medio Ambiente. | 3 | as first published, then each change: 28 December 2004 to 7 August 2015 | 2025-12-18 |
| `decreto-legislativo-2004-002/` | Decreto Legislativo 2/2004, de 30 de diciembre, del Gobierno de Aragón, por el que se aprueba el Texto Refundido de la Ley del Servicio Aragonés de Salud. | 3 | oldest version available, then each change: 15 January 2005 to 21 December 2016 | 2025-05-29 |
| `ley-2005-003/` | Ley 3/2005, de 12 de mayo, de creación de la entidad pública aragonesa del Banco de Sangre y Tejidos. | 4 | as first published, then each change: 7 June 2005 to 2 October 2021 | 2025-12-18 |
| `ley-2005-004/` | Ley 4/2005, de 14 de junio, sobre la casación foral Aragonesa. | 1 | as first published: 25 June 2005 | 2025-12-18 |
| `ley-2005-005/` | Ley 5/2005, de 14 de junio, de Ordenación del Sistema Universitario de Aragón. | 9 | as first published, then each change: 25 June 2005 to 27 August 2022 | 2025-12-18 |
| `decreto-legislativo-2005-001/` | Decreto Legislativo 1/2005, de 26 de septiembre, del Gobierno de Aragón, por el que se aprueba el texto refundido de las disposiciones dictadas por la Comunidad Autónoma de Aragón en materia de tributos cedidos. | 28 | oldest version available, then each change: 29 October 2005 to 8 July 2025 | 2025-07-17 |
| `ley-2005-007/` | Ley 7/2005, de 4 de octubre, de horarios comerciales y apertura de festivos. | 4 | as first published, then each change: 5 November 2005 to 16 May 2017 | 2025-12-18 |
| `ley-2005-009/` | Ley 9/2005, de 10 de octubre, de creación del Colegio Profesional de Educadoras y Educadores Sociales de Aragón. | 1 | as first published: 27 October 2005 | 2025-12-18 |
| `ley-2005-010/` | Ley 10/2005, de 11 de noviembre, de vías pecuarias de Aragón. | 6 | as first published, then each change: 13 December 2005 to 27 August 2022 | 2025-12-18 |
| `ley-2005-011/` | Ley 11/2005, de 28 de diciembre, reguladora de los espectáculos públicos, actividades recreativas y establecimientos públicos de la Comunidad Autónoma de Aragón. | 8 | as first published, then each change: 20 January 2006 to 10 August 2026 | 2026-10-02 |
| `ley-2006-005/` | Ley 5/2006, de 22 de junio, de tasas y precios públicos de la Comunidad Autónoma de Aragón. | 5 | oldest version available, then each change: 18 July 2006 to 23 October 2021 | 2023-12-26 |
| `ley-2006-009/` | Ley 9/2006, de 30 de noviembre, de Calidad Alimentaria de Aragón. | 4 | as first published, then each change: 14 December 2006 to 4 February 2016 | 2025-12-19 |
| `ley-2006-010/` | Ley 10/2006, de 30 de noviembre, de creación de la Reserva Natural Dirigida de las Saladas de Chiprana. | 2 | as first published, then each change: 14 December 2006 to 20 March 2012 | 2025-12-19 |
| `decreto-legislativo-2006-001/` | Decreto Legislativo 1/2006, de 27 de diciembre, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Comarcalización de Aragón. | 14 | oldest version available, then each change: 31 December 2006 to 1 January 2022 | 2024-11-21 |
| `decreto-legislativo-2006-002/` | Decreto Legislativo 2/2006, de 27 de diciembre, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Delimitación Comarcal de Aragón. | 2 | oldest version available, then each change: 31 December 2006 to 13 April 2019 | 2023-12-26 |
| `ley-2006-014/` | Ley 14/2006, de 27 de diciembre, de declaración del Parque Natural de los Valles Occidentales. | 2 | as first published, then each change: 19 January 2007 to 20 March 2012 | 2025-12-19 |
| `ley-2006-016/` | Ley 16/2006, de 28 de diciembre, de Protección y Defensa de los Consumidores y Usuarios de Aragón. | 6 | as first published, then each change: 28 February 2007 to 5 April 2019 | 2025-12-19 |
| `ley-2006-017/` | Ley 17/2006, de 29 de diciembre, de Medidas urgentes en el sector del transporte interurbano de viajeros por carretera de la Comunidad Autónoma de Aragón. | 2 | as first published, then each change: 31 December 2006 to 26 January 2014 | 2025-12-19 |
| `ley-2007-001/` | Ley 1/2007, de 27 de febrero, de Actividades Feriales Oficiales de Aragón. | 2 | as first published, then each change: 22 March 2007 to 6 May 2010 | 2025-12-19 |
| `ley-2007-002/` | Ley 2/2007, de 27 de febrero, de creación, por segregación, del Colegio Profesional de Biólogos de Aragón. | 1 | as first published: 22 March 2007 | 2025-12-19 |
| `ley-2007-004/` | Ley 4/2007, de 22 de marzo, de Prevención y Protección Integral a las Mujeres Víctimas de Violencia en Aragón. | 1 | as first published: 10 April 2007 | 2025-12-19 |
| `ley-2007-005/` | Ley 5/2007, de 17 de diciembre, de creación del Colegio Profesional de Dietistas-Nutricionistas de Aragón. | 1 | as first published: 1 January 2008 | 2025-12-19 |
| `ley-2007-006/` | Ley 6/2007, de 17 de diciembre, de creación del Colegio Profesional de Ortopédicos de Aragón. | 1 | as first published: 1 January 2008 | 2025-12-19 |
| `ley-2007-008/` | Ley 8/2007, de 29 de diciembre, de Medidas Tributarias de la Comunidad Autónoma de Aragón. | 1 | as first published: 1 January 2008 | 2025-12-19 |
| `ley-2008-002/` | Ley 2/2008, de 14 de mayo, de Reestructuración del Sector Público Empresarial de la Comunidad Autónoma de Aragón. | 2 | as first published, then each change: 24 May 2008 to 27 January 2009 | 2025-12-19 |
| `ley-2008-004/` | Ley 4/2008, de 17 de junio, de medidas a favor de las Víctimas del Terrorismo. | 3 | as first published, then each change: 3 July 2008 to 14 March 2023 | 2025-12-19 |
| `decreto-ley-2008-001/` | Decreto Ley 1/2008, de 30 de octubre, del Gobierno de Aragón, de medidas administrativas urgentes para facilitar la actividad económica en Aragón. | 7 | oldest version available, then each change: 4 November 2008 to 31 December 2024 | 2025-02-12 |
| `ley-2009-001/` | Ley 1/2009, de 30 de marzo, del Consejo Consultivo de Aragón. | 3 | as first published, then each change: 8 March 2009 to 2 October 2021 | 2026-10-14 |
| `decreto-ley-2009-001/` | Decreto-ley 1/2009, de 14 de abril, del Gobierno de Aragón, por el que se aprueba el Plan especial de dinamización del sector de la vivienda y se autoriza la prestación de avales por el Gobierno de Aragón | 1 | oldest version available: 18 April 2009 | 2023-12-26 |
| `decreto-ley-2009-002/` | Decreto-Ley 2/2009, de 12 de mayo, del Gobierno de Aragón, de medidas urgentes para la promoción del empleo. | 2 | oldest version available, then each change: 20 May 2009 to 20 March 2012 | 2023-12-26 |
| `ley-2009-005/` | Ley 5/2009, de 30 de junio, de Servicios Sociales de Aragón. | 5 | oldest version available, then each change: 11 July 2009 to 21 December 2016 | 2025-12-19 |
| `ley-2009-006/` | Ley 6/2009, de 6 de julio, de Centros de Ocio de Alta Capacidad de Aragón. | 1 | as first published: 18 July 2009 | 2025-12-19 |
| `ley-2009-009/` | Ley 9/2009, de 22 de diciembre, reguladora de los Concejos Abiertos. | 4 | as first published, then each change: 31 December 2009 to 3 February 2015 | 2025-12-19 |
| `ley-2009-011/` | Ley 11/2009, de 30 de diciembre, de la Cámara de Cuentas de Aragón. | 1 | as first published: 20 January 2010 | 2025-12-19 |
| `ley-2010-007/` | Ley 7/2010, de 18 de noviembre, de protección contra la contaminación acústica de Aragón. | 1 | as first published: 3 March 2011 | 2025-12-19 |
| `decreto-legislativo-2011-001/` | Decreto Legislativo 1/2011, de 22 de marzo, del Gobierno de Aragón, por el que se aprueba, con el título de «Código del Derecho Foral de Aragón», el Texto Refundido de las Leyes civiles aragonesas. | 10 | oldest version available, then each change: 23 April 2011 to 22 May 2025 | 2026-04-29 |
| `ley-2011-009/` | Ley 9/2011, de 24 de marzo, de mediación familiar de Aragón. | 2 | as first published, then each change: 8 April 2011 to 20 March 2012 | 2025-12-19 |
| `ley-2011-010/` | Ley 10/2011, de 24 de marzo, de derechos y garantías de la dignidad de la persona en el proceso de morir y de la muerte. | 1 | as first published: 7 July 2011 | 2025-12-19 |
| `decreto-ley-2011-001/` | Decreto-ley 1/2011, de 29 de noviembre, del Gobierno de Aragón, de medidas urgentes de racionalización del Sector Público Empresarial. | 2 | oldest version available, then each change: 5 December 2011 to 1 January 2014 | 2023-12-26 |
| `ley-2012-004/` | Ley 4/2012, de 26 de abril, de medidas urgentes de racionalización del sector público empresarial. | 3 | as first published, then each change: 11 May 2012 to 17 February 2017 | 2025-12-19 |
| `ley-2012-005/` | Ley 5/2012, de 7 de junio, de Estabilidad Presupuestaria de Aragón. | 3 | as first published, then each change: 19 June 2012 to 4 February 2016 | 2025-12-19 |
| `ley-2012-007/` | Ley 7/2012, de 4 de octubre, de medidas extraordinarias en el sector público de la Comunidad Autónoma de Aragón para garantizar la estabilidad presupuestaria. | 3 | as first published, then each change: 11 October 2012 to 19 January 2019 | 2025-12-19 |
| `ley-2012-008/` | Ley 8/2012, de 13 de diciembre, de autoridad del profesorado en la Comunidad Autónoma de Aragón. | 1 | as first published: 20 January 2013 | 2025-12-19 |
| `ley-2013-001/` | Ley 1/2013, de 7 de marzo, de Regulación y Coordinación de los Servicios de Prevención, Extinción de Incendios y Salvamento de Aragón. | 2 | as first published, then each change: 22 March 2013 to 26 January 2014 | 2025-12-19 |
| `ley-2013-003/` | Ley 3/2013, de 9 de mayo, de uso, protección y promoción de las lenguas y modalidades lingüísticas propias de Aragón. | 1 | as first published: 24 June 2013 | 2025-12-19 |
| `ley-2013-005/` | Ley 5/2013, de 20 de junio, de calidad de los Servicios Públicos de la Administración de la Comunidad Autónoma de Aragón. | 1 | as first published: 4 July 2013 | 2025-12-19 |
| `ley-2013-008/` | Ley 8/2013, de 12 de septiembre, de Coordinación de Policías Locales de Aragón. | 4 | as first published, then each change: 25 September 2013 to 11 July 2018 | 2025-12-19 |
| `ley-2013-009/` | Ley 9/2013, de 28 de noviembre, de Autoridad de Profesionales del Sistema Sanitario y de Servicios Sociales Públicos de Aragón. | 1 | as first published: 13 December 2013 | 2025-12-19 |
| `decreto-legislativo-2013-002/` | Decreto Legislativo 2/2013, de 3 de diciembre, del Gobierno de Aragón, por el que se aprueba el Texto Refundido de la Ley de creación del Consejo de Protección de la Naturaleza. | 1 | oldest version available: 14 December 2013 | 2023-12-26 |
| `decreto-legislativo-2013-003/` | Decreto Legislativo 3/2013, de 3 de diciembre, del Gobierno de Aragón por el que se aprueba el Texto Refundido de la Ley de regulación y fomento de la actividad industrial de Aragón. | 2 | oldest version available, then each change: 14 December 2013 to 27 August 2022 | 2023-12-26 |
| `ley-2013-010/` | Ley 10/2013, de 19 de diciembre, del Instituto Aragonés de Gestión Ambiental. | 4 | as first published, then each change: 10 January 2014 to 23 October 2021 | 2025-12-19 |
| `ley-2014-002/` | Ley 2/2014, de 23 de enero, de Medidas Fiscales y Administrativas de la Comunidad Autónoma de Aragón. | 6 | as first published, then each change: 26 January 2014 to 12 July 2024 | 2025-12-19 |
| `ley-2014-004/` | Ley 4/2014, de 26 de junio, de Fundaciones Bancarias de Aragón. | 1 | as first published: 16 July 2014 | 2025-12-19 |
| `ley-2014-005/` | Ley 5/2014, de 26 de junio, de Salud Pública de Aragón. | 3 | as first published, then each change: 16 July 2014 to 2 October 2021 | 2025-12-19 |
| `decreto-legislativo-2014-001/` | Decreto-Legislativo 1/2014, de 8 de julio, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Urbanismo de Aragón. | 7 | oldest version available, then each change: 20 November 2014 to 31 December 2024 | 2025-02-12 |
| `decreto-legislativo-2014-002/` | Decreto Legislativo 2/2014, de 29 de agosto, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Cooperativas de Aragón. | 3 | oldest version available, then each change: 10 September 2014 to 21 December 2022 | 2023-12-26 |
| `ley-2014-009/` | Ley 9/2014, de 23 de octubre, de Apoyo a las Familias de Aragón. | 1 | as first published: 6 November 2014 | 2025-12-19 |
| `ley-2014-010/` | Ley 10/2014, de 27 de noviembre, de Aguas y Ríos de Aragón. | 8 | as first published, then each change: 10 June 2015 to 27 August 2022 | 2025-12-19 |
| `ley-2014-011/` | Ley 11/2014, de 4 de diciembre, de Prevención y Protección Ambiental de Aragón. | 5 | as first published, then each change: 11 December 2014 to 2 April 2023 | 2025-12-19 |
| `ley-2014-012/` | Ley 12/2014, de 18 de diciembre, de medidas para la efectiva integración del Consorcio Aragonés Sanitario de Alta Resolución en el Servicio Aragonés de Salud. | 1 | as first published: 31 December 2014 | 2025-12-19 |
| `ley-2015-001/` | Ley 1/2015, de 12 de marzo, de Caza de Aragón. | 2 | as first published, then each change: 14 April 2015 to 23 February 2021 | 2025-12-19 |
| `ley-2015-003/` | Ley 3/2015, de 25 de marzo, de Cámaras Oficiales de Comercio, Industria y Servicios de Aragón. | 1 | as first published: 11 April 2015 | 2025-12-19 |
| `ley-2015-004/` | Ley 4/2015, de 25 de marzo, de Comercio de Aragón. | 2 | as first published, then each change: 11 April 2015 to 2 August 2017 | 2025-12-19 |
| `ley-2015-006/` | Ley 6/2015, de 25 de marzo, de Juventud de Aragón. | 2 | as first published, then each change: 11 April 2015 to 7 May 2023 | 2025-12-19 |
| `ley-2015-007/` | Ley 7/2015, de 25 de marzo, de Bibliotecas de Aragón. | 1 | as first published: 30 April 2015 | 2025-12-19 |
| `ley-2015-008/` | Ley 8/2015, de 25 de marzo, de Transparencia de la Actividad Pública y Participación Ciudadana de Aragón. | 10 | as first published, then each change: 10 July 2015 to 19 June 2024 | 2025-12-19 |
| `decreto-legislativo-2015-001/` | Decreto Legislativo 1/2015, de 29 de julio, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Espacios Protegidos de Aragón. | 2 | oldest version available, then each change: 7 August 2015 to 4 February 2016 | 2023-12-26 |
| `decreto-legislativo-2015-002/` | Decreto Legislativo 2/2015, de 17 de noviembre, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Ordenación del Territorio de Aragón. | 10 | oldest version available, then each change: 21 November 2015 to 31 December 2024 | 2025-08-28 |
| `decreto-ley-2015-003/` | Decreto-ley 3/2015, de 15 de diciembre, del Gobierno de Aragón, de medidas urgentes de emergencia social en materia de prestaciones económicas de carácter social, pobreza energética y acceso a la vivienda. | 4 | oldest version available, then each change: 18 December 2015 to 14 February 2019 | 2023-12-26 |
| `decreto-legislativo-2016-001/` | Decreto Legislativo 1/2016, de 26 de julio, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley del Turismo de Aragón. | 3 | oldest version available, then each change: 4 August 2016 to 17 July 2023 | 2023-12-26 |
| `decreto-ley-2016-002/` | Decreto-ley 2/2016, de 30 de agosto, de medidas urgentes para la ejecución de las sentencias dictadas en relación con los concursos convocados en el marco del Decreto 124/2010, de 22 de junio, y el impulso de la producción de energía eléctrica a partir de la energía eólica en Aragón. | 4 | oldest version available, then each change: 1 September 2016 to 31 December 2024 | 2025-02-12 |
| `ley-2016-009/` | Ley 9/2016, de 3 de noviembre, de reducción de la pobreza energética de Aragón. | 1 | as first published: 12 November 2016 | 2025-12-19 |
| `ley-2016-010/` | Ley 10/2016, de 1 de diciembre, de medidas de emergencia en relación con las prestaciones económicas del Sistema Público de Servicios Sociales y con el acceso a la vivienda en la Comunidad Autónoma de Aragón. | 7 | as first published, then each change: 1 January 2017 to 27 August 2022 | 2026-01-26 |
| `ley-2016-011/` | Ley 11/2016, de 15 de diciembre, de acción concertada para la prestación a las personas de servicios de carácter social y sanitario. | 1 | as first published: 21 December 2016 | 2025-12-19 |
| `ley-2017-001/` | Ley 1/2017, de 8 de febrero, de medidas de racionalización del régimen retributivo y de clasificación profesional del personal directivo y del resto del personal al servicio de los entes del sector público institucional de la Comunidad Autónoma de Aragón. | 2 | as first published, then each change: 17 February 2017 to 1 January 2020 | 2025-12-19 |
| `ley-2017-005/` | Ley 5/2017, de 1 de junio, de Integridad y Ética Públicas. | 2 | as first published, then each change: 6 July 2017 to 16 May 2023 | 2025-12-19 |
| `ley-2017-006/` | Ley 6/2017, de 15 de junio, de Cuentas Abiertas de Aragón. | 1 | as first published: 24 June 2017 | 2025-12-19 |
| `decreto-legislativo-2017-001/` | Decreto Legislativo 1/2017, de 20 de junio, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Montes de Aragón. | 2 | oldest version available, then each change: 1 July 2017 to 23 February 2021 | 2026-04-17 |
| `ley-2017-007/` | Ley 7/2017, de 28 de junio, de Venta Local de Productos Agroalimentarios en Aragón. | 1 | as first published: 2 August 2017 | 2025-12-19 |
| `ley-2017-009/` | Ley 9/2017, de 19 de octubre, por la que se regulan los servicios de asesoramiento y orientación jurídicos gratuitos de Aragón. | 1 | as first published: 30 November 2017 | 2025-12-19 |
| `ley-2017-010/` | Ley 10/2017, de 30 de noviembre, de régimen especial del municipio de Zaragoza como capital de Aragón. | 3 | as first published, then each change: 21 December 2017 to 15 January 2019 | 2025-12-20 |
| `ley-2018-001/` | Ley 1/2018, de 8 de febrero, de diálogo social y participación institucional en Aragón. | 1 | as first published: 22 February 2018 | 2025-12-20 |
| `ley-2018-003/` | Ley 3/2018, de 19 de abril, de creación del Colegio Profesional de Periodistas de Aragón. | 1 | as first published: 1 May 2018 | 2025-12-20 |
| `ley-2018-004/` | Ley 4/2018, de 19 de abril, de Identidad y Expresión de Género e Igualdad Social y no Discriminación de la Comunidad Autónoma de Aragón. | 2 | as first published, then each change: 8 May 2018 to 12 January 2019 | 2025-12-20 |
| `ley-2018-005/` | Ley 5/2018, de 19 de abril, del Taxi. | 2 | as first published, then each change: 8 June 2018 to 17 July 2023 | 2025-12-20 |
| `ley-2018-006/` | Ley 6/2018, de 28 de junio, del Voluntariado de Aragón. | 1 | as first published: 11 July 2018 | 2025-12-20 |
| `ley-2018-007/` | Ley 7/2018, de 28 de junio, de igualdad de oportunidades entre mujeres y hombres en Aragón. | 1 | as first published: 30 July 2018 | 2025-12-20 |
| `ley-2018-008/` | Ley 8/2018, de 28 de junio, de actualización de los derechos históricos de Aragón. | 5 | as first published, then each change: 29 June 2018 to 29 February 2020 | 2025-12-20 |
| `ley-2018-009/` | Ley 9/2018, de 28 de junio, de modificación de la ley 8/2013, de 12 de septiembre, de coordinación de policías locales de Aragón. | 1 | as first published: 11 July 2018 | 2025-12-20 |
| `ley-2018-011/` | Ley 11/2018, de 20 de septiembre, de creación del Colegio Profesional de Ingenieros en Informática de Aragón. | 2 | as first published, then each change: 4 October 2018 to 8 January 2021 | 2025-12-20 |
| `ley-2018-012/` | Ley 12/2018, de 20 de septiembre, de creación del Colegio Profesional de Ingenieros Técnicos en Informática de Aragón. | 1 | as first published: 4 October 2018 | 2025-12-20 |
| `ley-2018-013/` | Ley 13/2018, de 4 de octubre, de creación del Colegio de Economistas de Aragón por fusión de los Colegios Oficiales de Economistas de Aragón y de Titulados Mercantiles de Aragón. | 1 | as first published: 23 October 2018 | 2025-12-20 |
| `ley-2018-014/` | Ley 14/2018, de 8 de noviembre, de memoria democrática de Aragón. | 3 | as first published, then each change: 22 February 2019 to 19 June 2024 | 2026-03-17 |
| `ley-2018-016/` | Ley 16/2018, de 4 de diciembre, de la actividad física y el deporte de Aragón. | 2 | as first published, then each change: 20 December 2018 to 20 April 2022 | 2025-12-20 |
| `ley-2018-017/` | Ley 17/2018, de 4 de diciembre, de Investigación e Innovación de Aragón. | 1 | as first published: 20 December 2018 | 2025-12-20 |
| `ley-2018-018/` | Ley 18/2018, de 20 de diciembre, de igualdad y protección integral contra la discriminación por razón de orientación sexual, expresión e identidad de género en la Comunidad Autónoma de Aragón. | 1 | as first published: 12 January 2019 | 2025-12-20 |
| `decreto-ley-2019-002/` | Decreto-ley 2/2019, de 15 de enero, del Gobierno de Aragón, por el que se modifica el régimen de medidas en materia de incapacidad temporal del personal funcionario, estatutario y laboral del sector público de la Comunidad Autónoma de Aragón. | 1 | oldest version available: 19 January 2019 | 2023-12-26 |
| `decreto-ley-2019-003/` | Decreto-ley 3/2019, de 15 de enero, del Gobierno de Aragón, por el que se aprueban medidas urgentes en materia de retribuciones en el ámbito del sector público de la Comunidad Autónoma de Aragón. | 1 | oldest version available: 18 January 2019 | 2023-12-26 |
| `ley-2019-002/` | Ley 2/2019, de 21 de febrero, de aprendizaje a lo largo de la vida adulta en la Comunidad Autónoma de Aragón. | 1 | as first published: 26 March 2019 | 2025-12-20 |
| `decreto-ley-2019-007/` | Decreto-ley 7/2019, de 12 de marzo, del Gobierno de Aragón, de medidas urgentes en materia de transporte de viajeros mediante el arrendamiento de vehículos con conductor. | 1 | oldest version available: 16 March 2019 | 2023-12-26 |
| `ley-2019-005/` | Ley 5/2019, de 21 de marzo, de derechos y garantías de las personas con discapacidad en Aragón. | 1 | as first published: 10 July 2019 | 2025-12-20 |
| `ley-2019-007/` | Ley 7/2019, de 29 de marzo, de apoyo y fomento del emprendimiento y del trabajo autónomo en Aragón. | 2 | as first published, then each change: 2 May 2019 to 23 February 2021 | 2025-12-20 |
| `ley-2019-008/` | Ley 8/2019, de 29 de marzo, de creación de la Comarca Central. | 1 | as first published: 13 April 2019 | 2025-12-20 |
| `decreto-ley-2019-009/` | Decreto-ley 9/2019, de 8 de octubre, del Gobierno de Aragón, por el que se adoptan medidas extraordinarias y urgentes para el control de la población silvestre de conejo común (Oryctolagus cuniculus) en Aragón. | 2 | oldest version available, then each change: 12 October 2019 to 23 February 2021 | 2023-12-26 |
| `ley-2020-001/` | Ley 1/2020, de 9 de julio, por la que se establecen medidas excepcionales para el ejercicio 2020 en determinados tributos gestionados por la Comunidad Autónoma de Aragón. | 1 | as first published: 18 July 2020 | 2025-12-20 |
| `ley-2020-002/` | Ley 2/2020, de 22 de octubre, de Estadística de Aragón. | 1 | as first published: 31 October 2020 | 2026-02-23 |
| `ley-2020-003/` | Ley 3/2020, de 3 de diciembre, por la que se establece el régimen jurídico de alerta sanitaria para el control de la pandemia COVID-19 en Aragón. | 6 | as first published, then each change: 4 December 2020 to 16 September 2021 | 2025-12-20 |
| `decreto-ley-2021-001/` | Decreto-ley 1/2021, de 4 de enero, del Gobierno de Aragón, por el que se restablece el nivel de alerta sanitaria 3 agravado para el control de la pandemia COVID-19 en Aragón. | 1 | oldest version available: 4 January 2021 | 2023-12-26 |
| `ley-2021-001/` | Ley 1/2021, de 11 de febrero, de simplificación administrativa. | 5 | as first published, then each change: 23 February 2021 to 31 December 2024 | 2025-12-20 |
| `ley-2021-003/` | Ley 3/2021, de 20 de mayo, por la que se regula la Prestación Aragonesa Complementaria del Ingreso Mínimo Vital y el Servicio Público Aragonés de Inclusión Social. | 2 | as first published, then each change: 25 May 2021 to 1 August 2022 | 2026-01-26 |
| `decreto-ley-2021-003/` | Decreto-ley 3/2021, de 16 de junio, del Gobierno de Aragón, por el que se adoptan medidas urgentes y extraordinarias de gestión administrativa y económica de las ayudas incluidas en el Real Decreto-ley 5/2021, de 12 de marzo, de medidas extraordinarias de apoyo a la solvencia empresarial en respuesta a la pandemia de la COVID-19. | 1 | oldest version available: 21 June 2021 | 2024-05-07 |
| `ley-2021-005/` | Ley 5/2021, de 29 de junio, de Organización y Régimen Jurídico del Sector Público Autonómico de Aragón. | 5 | as first published, then each change: 3 July 2021 to 30 May 2023 | 2025-12-20 |
| `ley-2021-008/` | Ley 8/2021, de 9 de diciembre, de regulación del Impuesto Medioambiental sobre las Aguas Residuales. | 1 | as first published: 1 January 2022 | 2025-12-20 |
| `decreto-legislativo-2022-001/` | Decreto Legislativo 1/2022, de 6 de abril, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley del Presidente o Presidenta y del Gobierno de Aragón. | 1 | as first published: 21 April 2022 | 2026-10-02 |
| `decreto-ley-2022-002/` | Decreto-ley 2/2022, de 6 de abril, del Gobierno de Aragón, por el que se adoptan medidas urgentes y extraordinarias para agilizar la gestión de los fondos procedentes del instrumento europeo de recuperación (Next Generation EU-MRR) para la reactivación económica y social de la Comunidad Autónoma de Aragón. | 2 | as first published, then each change: 8 April 2022 to 1 January 2023 | 2025-12-20 |
| `decreto-ley-2022-003/` | Decreto-ley 3/2022, de 6 de abril, del Gobierno de Aragón, por el que se adoptan medidas excepcionales y urgentes en la contratación pública en Aragón. | 4 | as first published, then each change: 9 April 2022 to 30 October 2025 | 2025-12-20 |
| `ley-2022-002/` | Ley 2/2022, de 19 de mayo, de aplicación y desarrollo de la Ley 1/2021, de 11 de febrero, de simplificación administrativa. | 3 | as first published, then each change: 27 August 2022 to 30 May 2023 | 2025-12-20 |
| `ley-2022-003/` | Ley 3/2022, de 6 de octubre, de información geográfica de Aragón. | 1 | as first published: 26 October 2022 | 2025-12-20 |
| `ley-2022-004/` | Ley 4/2022, de 6 de octubre, de creación del Colegio Profesional de Higienistas Dentales de Aragón. | 1 | as first published: 26 October 2022 | 2025-12-20 |
| `ley-2022-005/` | Ley 5/2022, de 6 de octubre, Reguladora del Fondo Aragonés de Financiación Municipal. | 4 | as first published, then each change: 1 January 2023 to 19 June 2024 | 2025-12-20 |
| `ley-2022-006/` | Ley 6/2022, de 1 de diciembre, de creación del Colegio Profesional de Ópticos-Optometristas de Aragón. | 1 | as first published: 16 December 2022 | 2025-12-20 |
| `ley-2022-007/` | Ley 7/2022, de 1 de diciembre, de Economía Social de Aragón. | 1 | as first published: 21 December 2022 | 2025-12-20 |
| `decreto-legislativo-2023-001/` | Decreto Legislativo 1/2023, de 22 de febrero, por el que se aprueba el Texto Refundido de la Ley del Patrimonio de Aragón. | 1 | as first published: 4 March 2023 | 2025-12-20 |
| `ley-2023-006/` | Ley 6/2023, de 23 de febrero, de protección y modernización de la agricultura social y familiar y del patrimonio agrario de Aragón. | 2 | as first published, then each change: 2 April 2023 to 22 May 2025 | 2025-12-20 |
| `ley-2023-007/` | Ley 7/2023, de 23 de febrero, de medidas para la implantación y desarrollo en Aragón de tecnologías en la nube (tecnologías cloud). | 1 | as first published: 14 March 2023 | 2025-12-20 |
| `ley-2023-008/` | Ley 8/2023, de 9 de marzo, de Cultura de la Paz en Aragón. | 1 | as first published: 24 March 2023 | 2025-12-20 |
| `ley-2023-011/` | Ley 11/2023, de 30 de marzo, de uso estratégico de la contratación pública de la Comunidad Autónoma de Aragón. | 2 | as first published, then each change: 17 May 2023 to 28 November 2023 | 2025-12-20 |
| `ley-2023-013/` | Ley 13/2023, de 30 de marzo, de dinamización del medio rural de Aragón. | 1 | as first published: 18 April 2023 | 2025-12-20 |
| `ley-2023-014/` | Ley 14/2023, de 30 de marzo, de perros de asistencia en Aragón. | 1 | as first published: 17 July 2023 | 2025-12-20 |
| `decreto-legislativo-2023-002/` | Decreto Legislativo 2/2023, de 3 de mayo, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Subvenciones de Aragón. | 1 | as first published: 16 May 2023 | 2025-12-20 |
| `decreto-legislativo-2023-003/` | Decreto Legislativo 3/2023, de 17 de mayo, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Hacienda de la Comunidad Autónoma de Aragón. | 1 | as first published: 30 May 2023 | 2026-08-10 |
| `ley-2024-003/` | Ley 3/2024, de 13 de junio, de modificación del Código del Derecho Foral de Aragón en materia de capacidad jurídica de las personas. | 1 | as first published: 15 July 2024 | 2025-12-20 |
| `ley-2024-004/` | Ley 4/2024, de 28 de junio, del Sistema de Protección Civil y Gestión de Emergencias de Aragón. | 1 | as first published: 12 July 2024 | 2025-12-20 |
| `ley-2024-005/` | Ley 5/2024, de 19 de diciembre, de medidas de fomento de comunidades energéticas y autoconsumo industrial en Aragón. | 4 | as first published, then each change: 31 December 2024 to 19 March 2026 | 2026-03-19 |
| `ley-1986-008/` | Ley 8/1986, de 19 de diciembre, de Bibliotecas de Aragón. | 2 | as first published, then each change: 15 January 1987 to 30 April 2015; **repealed** 30 April 2015 by Ley 7/2015, de 25 de marzo (BOE-A-2015-5331) | 2025-12-17 |
| `ley-1989-009/` | Ley 9/1989, de 5 de octubre, de Ordenación de la Actividad Comercial en Aragón. | 12 | as first published, then each change: 1 January 1990 to 11 April 2015; **repealed** 11 April 2015 by Ley 4/2015, de 25 de marzo (BOE-A-2015-5328) | 2025-12-17 |
| `ley-1992-014/` | Ley 14/1992, de 28 de diciembre, de patrimonio agrario de la Comunidad Autónoma de Aragón y de medidas específicas de reforma y desarrollo agrario. | 4 | as first published, then each change: 28 January 1993 to 2 April 2023; **repealed** 2 April 2023 by Ley 6/2023, de 23 de febrero (BOE-A-2023-7735) | 2025-12-17 |
| `ley-1994-006/` | Ley 6/1994, de 30 de junio, de financiación agraria de la Comunidad Autónoma de Aragón. | 2 | as first published, then each change: 31 July 1994 to 2 April 2023; **repealed** 2 April 2023 by Ley 6/2023, de 23 de febrero (BOE-A-2023-7735) | 2025-12-17 |
| `ley-1997-003/` | Ley 3/1997, de 7 de abril, de Promoción de la Accesibilidad y Supresión de Barreras Arquitectónicas, Urbanísticas, de Transportes y de la Comunicación. | 2 | as first published, then each change: 8 May 1997 to 10 July 2019; **repealed** 10 July 2019 by Ley 5/2019, de 21 de marzo (BOE-A-2019-7785) | 2025-12-18 |
| `decreto-legislativo-2000-001/` | Decreto Legislativo 1/2000, de 29 junio, del Gobierno de Aragón, por el que se aprueba el texto refundido de la Ley de Hacienda de la Comunidad Autónoma de Aragón. | 11 | oldest version available, then each change: 1 July 2000 to 30 May 2023; **repealed** 30 May 2023 by Decreto Legislativo 3/2023, de 17 de mayo (BOE-A-2023-14052) | 2023-12-26 |
| `decreto-legislativo-2001-002/` | Decreto Legislativo 2/2001, de 3 julio, del Gobierno de Aragón, por el que se aprueba el Texto Refundido de la Ley de la Administración de la Comunidad Autónoma de Aragón. | 10 | oldest version available, then each change: 21 July 2001 to 2 October 2021; **repealed** 2 October 2021 by Ley 5/2021, de 29 de junio (BOE-A-2021-12701) | 2024-04-30 |
| `ley-2002-005/` | Ley 5/2002, de 4 de abril, de Caza, de Aragón. | 7 | as first published, then each change: 7 May 2002 to 14 April 2015; **repealed** 14 April 2015 by Ley 1/2015, de 12 de marzo (BOE-A-2015-5291) | 2025-12-18 |
| `ley-2002-016/` | Ley 16/2002, de 28 de junio, de Educación Permanente de Aragón. | 3 | as first published, then each change: 9 July 2002 to 26 March 2019; **repealed** 26 March 2019 by Ley 2/2019, de 21 de febrero (BOE-A-2019-5575) | 2025-12-18 |
| `ley-2002-030/` | Ley 30/2002, de 17 de diciembre, de Protección Civil y Atención de Emergencias de Aragón. | 7 | as first published, then each change: 31 January 2003 to 12 July 2024; **repealed** 12 July 2024 by Ley 4/2024, de 28 de junio (BOE-A-2024-15350) | 2025-12-18 |
| `ley-2004-006/` | Ley 6/2004, de 9 de diciembre, por la que se establecen medidas en materia de expropiación forzosa para actuaciones de mejora y creación de regadíos. | 2 | as first published, then each change: 25 December 2005 to 2 April 2023; **repealed** 2 April 2023 by Ley 6/2023, de 23 de febrero (BOE-A-2023-7735) | 2025-12-18 |
| `ley-2006-015/` | Ley 15/2006, de 28 de diciembre, de Montes de Aragón. | 8 | as first published, then each change: 29 January 2007 to 1 July 2017; **repealed** 1 July 2017 by Decreto Legislativo 1/2017, de 20 de junio (BOA-d-2017-90392) | 2025-12-19 |
| `ley-2009-002/` | Ley 2/2009, de 11 de mayo, del Presidente y del Gobierno de Aragón. | 8 | as first published, then each change: 8 June 2009 to 21 April 2022; **repealed** 21 April 2022 by Decreto Legislativo 1/2022, de 6 de abril (BOE-A-2022-7004) | 2025-12-19 |
| `ley-2009-004/` | Ley 4/2009, de 22 de junio, de Ordenación del Territorio de Aragón. | 5 | as first published, then each change: 1 July 2009 to 21 November 2015; **repealed** 21 November 2015 by Decreto Legislativo 2/2015, de 17 de noviembre (BOA-d-2015-90603) | 2025-12-19 |
| `ley-2011-001/` | Ley 1/2011, de 10 de febrero, de convenios de la Comunidad Autónoma de Aragón. | 2 | as first published, then each change: 26 March 2011 to 2 October 2021; **repealed** 2 October 2021 by Ley 5/2021, de 29 de junio (BOE-A-2021-12701) | 2025-12-19 |
| `ley-2011-003/` | Ley 3/2011, de 24 de febrero, de medidas en materia de Contratos del Sector Público de Aragón. | 14 | as first published, then each change: 10 May 2011 to 17 May 2023; **repealed** 17 May 2023 by Ley 11/2023, de 30 de marzo (BOE-A-2023-10876) | 2025-12-19 |
| `decreto-legislativo-2013-004/` | Decreto Legislativo 4/2013, de 17 de diciembre, del Gobierno de Aragón, por el que se aprueba el Texto Refundido de la Ley del Patrimonio de Aragón. | 5 | oldest version available, then each change: 1 January 2014 to 4 March 2023; **repealed** 4 March 2023 by Decreto Legislativo 1/2023, de 22 de febrero (BOE-A-2023-7507) | 2024-11-21 |
| `ley-2015-005/` | Ley 5/2015, de 25 de marzo, de Subvenciones de Aragón. | 7 | as first published, then each change: 10 May 2015 to 16 May 2023; **repealed** 16 May 2023 by Decreto Legislativo 2/2023, de 3 de mayo (BOE-A-2023-12919) | 2025-12-19 |
| `decreto-ley-2016-001/` | Decreto-Ley 1/2016, de 17 de mayo, del Gobierno de Aragón, sobre acción concertada para la prestación a las personas de servicios de carácter social y sanitario. | 2 | oldest version available, then each change: 20 May 2016 to 21 December 2016; **repealed** 21 December 2016 by Ley 11/2016, de 15 de diciembre (BOE-A-2017-491) | 2023-12-26 |
| `decreto-ley-2020-001/` | Decreto-Ley 1/2020, de 25 de marzo, del Gobierno de Aragón, por el que se adoptan medidas urgentes para responder al impacto generado por el COVID-19 en la Comunidad Autónoma de Aragón. | 2 | oldest version available, then each change: 25 March 2020 to 23 February 2021; **repealed** 23 February 2021 by Ley 1/2021, de 11 de febrero (BOE-A-2021-4247) | 2026-05-12 |
| `decreto-ley-2020-002/` | Decreto-ley 2/2020, de 28 de abril, del Gobierno de Aragón, por el que se adoptan medidas adicionales para responder al impacto generado por el COVID-19 en la Comunidad Autónoma de Aragón. | 2 | oldest version available, then each change: 29 April 2020 to 23 February 2021; **repealed** 23 February 2021 by Ley 1/2021, de 11 de febrero (BOE-A-2021-4247) | 2026-05-12 |
| `decreto-ley-2020-004/` | Decreto-ley 4/2020, de 24 de junio, del Gobierno de Aragón, por el que se adoptan medidas urgentes y extraordinarias para el impulso de la Estrategia Aragonesa para la Recuperación Social y Económica. | 4 | oldest version available, then each change: 25 June 2020 to 23 February 2021; **repealed** 23 February 2021 by Ley 1/2021, de 11 de febrero (BOE-A-2021-4247) | 2026-10-20 |
| `decreto-ley-2020-005/` | Decreto-ley 5/2020, de 29 de junio, del Gobierno de Aragón, por el que se regula la Prestación Aragonesa Complementaria del Ingreso Mínimo Vital y el Servicio Público Aragonés de Inclusión Social. | 2 | oldest version available, then each change: 30 June 2020 to 25 May 2021; **repealed** 25 May 2021 by Ley 3/2021, de 20 de mayo (BOE-A-2021-10673) | 2026-05-12 |
| `decreto-ley-2020-007/` | Decreto-ley 7/2020, de 19 de octubre, del Gobierno de Aragón, por el que se establece el régimen jurídico de alerta sanitaria para el control de la pandemia COVID-19 en Aragón. | 4 | oldest version available, then each change: 19 October 2020 to 4 December 2020; **repealed** 4 December 2020 by Ley 3/2020, de 3 de diciembre (BOE-A-2021-2767) | 2026-05-12 |
| `decreto-ley-2020-008/` | Decreto-ley 8/2020, de 21 de octubre, del Gobierno de Aragón, por el que se modifican niveles de alerta y se declara el confinamiento de determinados ámbitos territoriales en la Comunidad Autónoma de Aragón. | 2 | oldest version available, then each change: 21 October 2020 to 4 December 2020; **repealed** 4 December 2020 by Ley 3/2020, de 3 de diciembre (BOE-A-2021-2767) | 2026-05-12 |
| `decreto-ley-2020-009/` | Decreto-ley 9/2020, de 4 de noviembre, del Gobierno de Aragón, por el que se modifica el Decreto-ley 7/2020, de 19 de octubre, del Gobierno de Aragón, por el que se establece el régimen jurídico de la alerta sanitaria para el control de la pandemia COVID-19 en Aragón. | 2 | oldest version available, then each change: 5 November 2020 to 4 December 2020; **repealed** 4 December 2020 by Ley 3/2020, de 3 de diciembre (BOE-A-2021-2767) | 2026-05-12 |

## Source

The consolidated legislation of the Agencia Estatal Boletín Oficial del Estado (BOE), through its open-data API, <https://www.boe.es/datosabiertos/api/legislacion-consolidada>. For each consolidated norm it gives every block of the text (article, disposition, annex, heading) with every version of that block, the day each version took effect (fecha_vigencia) and the norm that made it (id_norma). Each version here is the whole text as it stood on one of those days. The last column above is the BOE's own last-update date for the consolidated text.

## Dates

- Each commit is dated at **noon, Europe/Madrid, on the day the change took effect**: the fecha_vigencia the BOE gives the new block versions.
- A day on which the BOE records a new block version that changes no words is not a version here.
- Block versions with no in-force date (the BOE's 99999999, a date not yet fixed) are left out.
- An act's first commit is its first publication when the BOE's earliest text is the act as enacted; otherwise it is the oldest version the BOE holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 bis; `da-01.md` the Disposición adicional primera, `dt-` transitional, `dd-` repealing and `df-` final dispositions (`-unica` for "única"); `preambulo.md` the preamble, `firma.md` the signature, `anexo-*.md` the annexes. The book, title, chapter and section headings sit at the top of the file of the article that follows them. One paragraph per line; a table one line per row, cells separated by ` | `.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the BOE's own text of that day, rebuilt from the source XML by a separate reader, and every file's text appears in it.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the norm that changed the text (a law, a decree-law, a ruling of the Constitutional Court), named by its title and BOE identifier, with an e-mail address that cannot exist (`<boe id>@boe.es.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. Only the texts published in the official journals are authentic. The history starts with the oldest text the BOE consolidates for each norm. Only the norms listed above are included; norms the BOE does not consolidate are not.
