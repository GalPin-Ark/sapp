<script>
  import {
    Button, Card, CardBody, CardFooter, CardHeader,
    CardImg, CardSubtitle, CardText, CardTitle
  } from "sveltestrap";
</script>
<style>
	h1, figure, p {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}

	figure {
		margin: 0 0 1em 0;
	}

	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	p {
		margin: 1em auto;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}
</style>

<svelte:head>
	<title>Sapper project template</title>

</svelte:head>

<Card class="mb-3">
  <CardHeader>
    <CardTitle>Card title</CardTitle>
  </CardHeader>
  <CardBody>
    <CardSubtitle>Card subtitle</CardSubtitle>
    <CardText>
      Some quick example text to build on the card title
      and make up the bulk of the card's content.
    </CardText>
    <Button on:click={()=> alert("button")}>Button</Button>
  </CardBody>
  <CardFooter>Footer</CardFooter>
</Card>

<figure>
	<img alt='Borat' src='great-success.png'>
	<figcaption>HIGH FIVE!</figcaption>
</figure>

<p><strong>Try editing this file (src/routes/index.svelte) to test live reloading.</strong></p>
