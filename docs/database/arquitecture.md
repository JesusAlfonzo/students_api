### 🏢 Diseño de la Base de Datos (DBML)

```dbml
Table Users {
  id int [pk]
  first_name varchar
  last_name varchar
  email varchar
  password varchar
}

Table Roles {
  id int [pk]
  name varchar
  description varchar
}

Table User_Roles {
  id int [pk]
  user_id int [ref: > Users.id]
  role_id int [ref: > Roles.id]
}

Table Subjects {
  id int [pk]
  name varchar
  description varchar
}

Table Evaluations {
  id int [pk]
  subject_id int [ref: > Subjects.id]
  name varchar
  description varchar
  score float
  participated bool
}

Table Students_info {
  id int [pk]
  user_id int [ref: - Users.id]
  phone varchar 
  address varchar
  identification varchar 
  gender bool
  disability bool
  record int
  birthday date
  birthplace varchar
  status bool
}

Table Teachers_info {
  id int [pk]
  user_id int [ref: - Users.id]
  phone varchar 
  address varchar
  identification varchar 
  status bool
}

Table Registration {
  id int [pk]
  user_id int [ref: > Users.id]
  subject_id int [ref: > Subjects.id]
  date date
}