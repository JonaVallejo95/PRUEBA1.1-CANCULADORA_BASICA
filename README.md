ESTE CODIGO CONSTA DE UNA CALCULADORA BASICA 
lass MainActivity : AppCompatActivity() {    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

                val n1= findViewById<EditText>(R.id.txt_n1)
                val n2= findViewById<EditText>(R.id.txt_n2)
                val r= findViewById<TextView>(R.id.txt_respuesta)
                val btn_sumar= findViewById<Button>(R.id.btn_suma)
                val btn_resta= findViewById<Button>(R.id.btn_resta)
                val btn_multiplicacion= findViewById<Button>(R.id.bnt_multip)
                val btn_division= findViewById<Button>(R.id.btn_division)

                btn_sumar.setOnClickListener {
                    r.setText(
                        "La suma es:"+(n1.text.toString().toInt()+n2.text.toString().toInt())
                    )
                }

                btn_resta.setOnClickListener {
                    r.setText(
                        "La resta es:"+(n1.text.toString().toInt()-n2.text.toString().toInt())
                    )
                }
                btn_multiplicacion.setOnClickListener {
                    r.setText(
                        "La multiplicacion es:"+(n1.text.toString().toInt()*n2.text.toString().toInt())
                    )
                }
                btn_division.setOnClickListener {
                    r.setText(
                        "La division es:"+(n1.text.toString().toInt()/n2.text.toString().toInt())
                    )
                }
            }

        }
