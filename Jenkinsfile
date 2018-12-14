pipeline
{
    agent 
    {
        node 
		{
            label 'slave-azure' 
        }
    }

    stages
    {
		stage ('HelloWorld') 
		{
			agent
			{
			 	docker { image 'idelala1/prueba' }
			}
			steps
			{
				echo 'Hello World'
			}
			post
			{
				success
				{
					echo 'Se ha saludado correctamente'
				}
				failure
				{
					echo 'Se ha producido error en el saludo'
				}
			}
		}
		
		stage ('MVN compile')
		{
			agent
			{
				docker { image 'idelala1/prueba' }
			}
			steps
			{
				script { libreria.compile 'prueba' }
			}
			post
			{
				success
				{
					echo 'Se ha descargado el repositorio'
				}
				failure
				{
					echo 'Se ha producido error en el saludo'
				}
			}
		}

    }
}
