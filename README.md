# Sticky Footer + Vertical Center

In several web projects we need to develop a fixed footer and a login screen. Considering this need, this code was written to serve as a basis for projects that include scenarios like this.

## CSS

```css
html, 
body {
	margin: 0;
	padding: 0;
	height: 100%;
}

.page-container {
	display: table;
	table-layout: fixed;
	width: 100%;
	height: 100%;
	height: auto\9; /* IE 8 Hack */
	min-height: 100%;
	position: relative;
}

.page-content {
	display: table-row;
	height: 100%;
}

.header,
.footer {
	display: table-row;
	height: 1px;
}

.vertical-center {
	height: 100%;
}

.vertical-center .page-content {
	display: table-cell;
	vertical-align: middle;
}
```

## HTML

### Sticky Footer WITH Header

```html
<!-- PAGE CONTAINER - Begin -->
<div class="page-container">

	<!-- HEADER - Begin -->
	<div class="header">
		<p>Header</p>
	</div>
	<!-- HEADER - End -->

	<!-- PAGE CONTENT - Begin -->
	<div class="page-content">

		<!-- MAIN - Begin -->
		<div class="main">
			<p>Main</p>
		</div>
		<!-- MAIN - End -->
	
	</div>
	<!-- PAGE CONTENT - End -->
	
	<!-- FOOTER - Begin -->
	<div class="footer">
		<p>Footer</p>
	</div>
	<!-- FOOTER - End -->

</div>
<!-- PAGE CONTAINER - End -->
```

### Sticky Footer + Vertical Center WITH Header

```html
<!-- VERTICAL CENTER - Begin -->
<div class="vertical-center">

	<!-- PAGE CONTAINER - Begin -->
	<div class="page-container">

		<!-- HEADER - Begin -->
		<div class="header">
			<p>Header</p>
		</div>
		<!-- HEADER - End -->

		<!-- PAGE CONTENT - Begin -->
		<div class="page-content">

			<!-- MAIN - Begin -->
			<div class="main">
				<p>Main</p>
			</div>
			<!-- MAIN - End -->
		
		</div>
		<!-- PAGE CONTENT - End -->
		
		<!-- FOOTER - Begin -->
		<div class="footer">
			<p>Footer</p>
		</div>
		<!-- FOOTER - End -->

	</div>
	<!-- PAGE CONTAINER - End -->

</div>
<!-- VERTICAL CENTER - End -->
```

### Sticky Footer WITHOUT Header

```html
<!-- PAGE CONTAINER - Begin -->
<div class="page-container">

	<!-- PAGE CONTENT - Begin -->
	<div class="page-content">

		<!-- MAIN - Begin -->
		<div class="main">
			<p>Main</p>
		</div>
		<!-- MAIN - End -->
	
	</div>
	<!-- PAGE CONTENT - End -->
	
	<!-- FOOTER - Begin -->
	<div class="footer">
		<p>Footer</p>
	</div>
	<!-- FOOTER - End -->

</div>
<!-- PAGE CONTAINER - End -->
```


### Sticky Footer + Vertical Center WITHOUT Header

```html
<!-- VERTICAL CENTER - Begin -->
<div class="vertical-center">

	<!-- PAGE CONTAINER - Begin -->
	<div class="page-container">
		
		<!-- PAGE CONTENT - Begin -->
		<div class="page-content">

			<!-- MAIN - Begin -->
			<div class="main">
				<p>Main</p>
			</div>
			<!-- MAIN - End -->
		
		</div>
		<!-- PAGE CONTENT - End -->
		
		<!-- FOOTER - Begin -->
		<div class="footer">
			<p>Footer</p>
		</div>
		<!-- FOOTER - End -->

	</div>
	<!-- PAGE CONTAINER - End -->

</div>
<!-- VERTICAL CENTER - End -->
```