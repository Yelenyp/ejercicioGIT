# ejercicioGIT
proyecto clase 2 github TEch Academy
ines yeleny piedrahita marquez

examen.html
Examen.html

Punto 2.

<script>
var numero =5;
var factorial =1;
for (var i=numero; i>=1; i++)
{
    factorial = factorial*i;
}
console.log (factorial);
</script>

Punto 3 Par -impar
<script>
<function parlmpar( numero){
    var resultado =";
    if(numero%2 ==0) {
        resultado = 'Par';
    }else{
    resultado = 'impar';
    }
        {
            Console.log(resultado);
            return resultado;
        }
        
    }
}
<script>

 
    Punto 4
    <script tipye= "text/javascript">
        function palindromo(cadena) {
<Var>resultado = "La cadena\""+cadena+"\"\n";
    <var> cadenaOriginal = cadena.toLowerCase();
        var letrasEspacios =cadenaOriginal.split("");
        var cadenaSinEspacios = "";
        for (i in letrasEspacios) {
            if(letrasEspacios[i] != ""){
                cadenaSinEspacios +=letrasEspacios[i];
            }
            }
    Var letras =cadenaSinEspacios.split("");
    var letrasReves = cadenaSinEspacios.split("").reverse();
    
    var iguales = true;
    for(i in letras) {
        if(letras[i] ==letrasReves[i]){

        }
        Else [iguales = false;
    }
}
if (iguales) {
    resultado += "es un palindromo";
}

else {
    resultado += "no es palíndromo";
}

return resultado;
}
alert(palindromo("la ruta nos apaorto otro paso natural"));
alert(palindromo("Esta frase no se parece a ningun palindromo"));
</script>
    
--Punto 5 

<script>
    namespace Travel.DTO.Cliente
{
    public class Persona
    {
        private int edad; // { get; set; }
        private string nombre; // { get; set; }
       
        public string Nombre { get => nombre; set => nombre = value; }
        public int Edad { get => edad; set => edad = value; }
        public Persona(string Nombre, int Edad)
        {
            this.nombre = Nombre;
            this.edad = Edad;
        }

        public virtual string objDetalles()
        {
            string respuesta = "nombre:" + this.nombre + "edad:" + this.edad.ToString();
            Console.WriteLine(respuesta);
            return respuesta;
            
        }

    }


    public class Estudiante : Persona{
   private double calificacion { get; set; }
        public double Calificacion { get => calificacion; set => calificacion = value; }

        public Estudiante(string Nombre, int edad, double califi) {
            this.Nombre = Nombre;
            this.Edad = edad;
            this.calificacion = califi;
        }
        public  override string objDetalles()
        {
            //Console.log("nombre:" + this.nombre + "edad:" edad.toString() + "Calificacion: " + calificacion.toString());
            string respuesta = "nombre:" + this.Nombre + "edad:" + this.Edad.ToString() + "Calificacion: " + calificacion.ToString();
            Console.WriteLine(respuesta);
            return respuesta;
        }
    }

    public class Profesor : Persona
    {
        private string asignatura; //{ get; set; }
        private int nivel; // { get; set; }

            public string Asignatura { get => asignatura; set => asignatura = value; }
            public int Nivel { get => nivel; set => nivel = value; }
            public Profesor (string Nombre, int Edad, string Asignatura, int Nivel)
            {
                this.Nombre = Nombre;
                this.Edad = Edad;
                this.asignatura = Asignatura;
                this.nivel = Nivel;
            }
        public override string objDetalles()
        {
            
            string respuesta = "nombre:" + this.Nombre + "edad:" + this.Edad.ToString() + "asignatura: " + asignatura.ToString() + "nivel: " + nivel.ToString();
            Console.WriteLine(respuesta);
            return respuesta;
        }
    }
    public class Grupo {
        private Profesor profesor;
        private double promedio ;
        private List<Estudiante> students;
        public Grupo(Profesor profe, List<Estudiante> listEstudiantes) {
            this.profesor = profe;
            this.students = listEstudiantes;

        }
        public void Calificar() {
            foreach (var item in students) {
                Random ran = new Random();

                item.Calificacion = ran.Next(0, 10);
            }
        }
        public double Promedio() {
            double resultado = 0;
            foreach (var item in students) {
                resultado += item.Calificacion;
            }
            return resultado/ students.Count;
        }
        public void objDetalles()
        {
            profesor.objDetalles();
            foreach (var item in this.students) {
                item.objDetalles();
            }
           
        }

        public void ArregloEstudiantes() {
            List<Estudiante> estudiantes = new List<Estudiante>();
            estudiantes.Add(new Estudiante("Caros Sanchez", 69,0));
            estudiantes.Add(new Estudiante("Yeleny", 69, 0));
            estudiantes.Add(new Estudiante("Juan", 20, 0));
            estudiantes.Add(new Estudiante("Maria", 16, 0));
            estudiantes.Add(new Estudiante("Andres", 60, 0));
            estudiantes.Add(new Estudiante("mARLA", 70, 0));
        }
    }



    
}
</script>
    
