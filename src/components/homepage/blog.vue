<template>
  <div class="blog">
    <div class="u-container">
	  <div class="u-row u-align-items-center">
		<a href="/regatta-group" class="u-col-4">
		    <picture>
				<source srcset="https://cdn.craghoppers.com/img/SS22/UK/homepage/blog-spot/02-feb/08/QGC-Blog.jpeg" media="(max-width: 768px)" />
				<img src="https://cdn.craghoppers.com/img/SS22/UK/homepage/blog-spot/02-feb/08/QGC-Blog.jpeg" alt="Blog Image" class="u-img-thumbnail" />
			</picture>
		</a>
		<div class="u-col-8">
			<h2>BLOG</h2>
			<h3>PLANTING TREES WITH THE QUEEN'S GREEN CANOPY</h3>
			<p>As part of The Regatta Group’s wider sustainability programme, Craghoppers, along with Regatta and Dare2b, is a platinum supporter of The Queen’s Green Canopy (QGC). This is a unique tree planting initiative, created in celebration of Her Majesty’s Platinum Jubilee in June this year, encouraging everyone all over the country to #PlantaTreefortheJubilee.</p>
			<a href="/regatta-group" class="link">Find Out More ></a>
		</div>
	  </div>
	</div>
  </div>
</template>

<script>
export default {
  name: "Blog",
  props: {},
};
</script>

<style scoped lang="scss">
	.blog {
		background-color: #dddddd;
		padding: 1.5rem 0;
		h2 {
			font-size: 1rem;
		}
		h3 {
			font-size: 1.5rem;
		}
		p {
			font-size: 0.8rem;
		}
		.link {
			color: blue;
			text-decoration: underline;
			margin-bottom: 0;
		}
	}
	.u-container {
		width: 100%;
		padding-right: var(--bs-gutter-x, 0.75rem);
		padding-left: var(--bs-gutter-x, 0.75rem);
		margin-right: auto;
		margin-left: auto;
	}
	@media (min-width: 576px) {
		.u-container {
			max-width: 540px;
		}
	}
	@media (min-width: 768px) {
		.u-container {
			max-width: 720px;
		}
	}
	@media (min-width: 992px) {
		.u-container {
			max-width: 960px;
		}
	}
	@media (min-width: 1200px) {
		.u-container {
			max-width: 1140px;
		}
	}
	.u-{
		&row {
			--bs-gutter-x: 1.5rem;
			--bs-gutter-y: 0;
			display: flex;
			flex-wrap: wrap;
			margin: 0;
		}
		&row > * {
			flex-shrink: 0;
			width: 100%;
			max-width: 100%;
			padding-right: calc(var(--bs-gutter-x) * 0.5);
			padding-left: calc(var(--bs-gutter-x) * 0.5);
			margin-top: var(--bs-gutter-y);
		}
		&col-4 {
			flex: 0 0 auto;
			width: 33.33333333%;
		}
		&col-8 {
			flex: 0 0 auto;
			width: 66.66666667%;
		}
		&align-items-center {
			align-items: center;
		}
		&img-thumbnail {
			display: block;
			width: 100%;
			padding: 0.25rem;
			background-color: #fff;
			border: 1px solid #dee2e6;
			border-radius: 0.25rem;
			max-width: 100%;
			height: auto;
		}
	}
</style>