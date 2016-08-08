Browserify
	permite modularizar la logia de javascript y depsues terminarlo en un solo archivo js
	bundle de dependencias tanto nuestras como de terceros
	scripts: 
		build browserigy app.sj >build.js -t babelify
Babelify
	tranpilar nuestro codigo de javascript ecms6, jsx a javascript comun que corre en cualqueira de los browsers

Props
	getDefaultProps
		se pueden definir porps por defecto
State
	setState()
		metodo de cada componente(paso objeto con nuevas propiedades y lo mezcla ocn las anteriores q tenia)

		llama al metodo render
		llamarlo lo menos posible 
		setState(nuevosDatos, callback)

		setInitilaState

		los padres tenga state

		ecmascirpt6 (constructor)
		va un objeto tipo Json en el state
		no van datos calcualdos
		no tener otros components
		datos duplicados de las props
Ciclo de vida
	Mounting
		componentWillMount()
		componentDidMount()
	Updating
		coomponentWillReceiveProps(nextProps)
		shouldComponentUpdate(nextProps,nextState)
		componentWillUpdate(nextProps,nextState)
		componentDidUpdate()
	Unmounting
		componentWillUnmount()
			para liberar memoria
Mixins
	compartir funcionaldiades entre components
	no disponibles para ecmacript6

EvenHandler como el usuario actua con el navegador
	onClick={this.onClick(funcionq se va ejecutar)}
	this.onClick.bind(this) Para q no tome windows
uid
	para crear id unicos libreria npm

realtiem app
	nos referimos a velocidad
	actualizaicon de datos latenica mininma
	datos actualizar uniformemente sin accion usuario
	rapida
	auto-autoactizable
	Authbolling
		cada tiempo se pide por neuvo datos (serTimeout)
		setInterval(...,5000)
	Serverpush
		servidor manda datos sin q el cliente lo pida(guillermo Raunch)
	State reconciliation
	Sesiones invalidad
	Cambio Usuario
	Deltas muy grandes
	Inicial load
	"single page app"
		Hibrido (usar render tanto en el backend como en el frontend)
		server side rendering
		client side rendering
	Sepuede usar componentes tanto del backend como del fronend

	Isomorphic
		reutilizar codigo tanto en el backend como en el frontend
		reutilizar las rutas

	Servidro realtime express
		express socket.io socket.io-client babel
__dirnmae
	para obtener el valor de la carpeta donde nos encontramos ubicados
Animaciones react.js
	react/addons
		ahi q incluir para usar las animaciones
		Reac.addons.CSSTransitionGroup;(permite dar y crear clases )
SuperAgent
Fetch
	se peuden usar para hacer las peticiones al servidor

Rutas
	react-router: coomponente que nos premite hacer el maanjeo de rutas frontend como backend
	Permite hacer isomorficas las apps

USAR COLBAT2 PARA SUBLIME ver merjo todo
Ajax
	$.ajax({
		url: '',
		dataType: 'jsonp',
		jsonpCallback: 'jsonFlcikrFeed',
		cache: false,
		context: this,
		success: function(){
			console.log('fetch ok');
			this.imagelist = data.items;
			this.trigger(this.imagelist);
			
	}
	})