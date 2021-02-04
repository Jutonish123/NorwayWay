<template>
	<div class="background-image">
		<div class="wrapper center">
			<div class="logo">
				<p>Your<span class="blue">way</span></p>
			</div>
			<div class="navigation">
				<router-link class="navigation-link" to="#">Авиабилеты</router-link>
				<router-link class="navigation-link" to="#">Туры</router-link>
				<router-link class="navigation-link" to="#">Проживание</router-link>
				<router-link class="navigation-link" to="#">Полезные статьи</router-link>
				<router-link class="navigation-link" to="#">Контакты</router-link>
			</div>
      <form>
        <div class="input-field">
          <input id="search" type="search" required>
          <label class="label-icon" for="search">
            <button type="submit" class="search-button">
              <i class="material-icons">search</i>
            </button>
          </label>
        </div>
      </form>
		</div>
		<div class="pageTitle center">
			<div class="title">
				<h1>Великолепные Фьорды <br> Норвегии</h1>
			</div>
      <a href="#" class="learn_link">
        <p>Узнайте больше</p>
      </a>
		</div>
	</div>
</template>
<script>

export default {
	name: 'Header',
}

</script>

<style lang="sass" scoped>

@import '../assets/style/variables'

.background-image
	background: url(../assets/img/Rectangle.jpg) no-repeat
	background-size: 100%

.wrapper
	color: $white
	display: flex
	justify-content: space-between
	padding-top: 60px

.logo p
	font-weight: 400
	font-size: 24px

.blue
	color: #6CC5D9
	font-size: 24px

.navigation
	&-link
		text-decoration: none
		color: $white
		font-size: 18px
		position: relative
		transition: 1s all linear
		display: inline-block
		&:after
			position: absolute
			content: ''
			height: 1px
			width: 0
			left: 0
			bottom: 0
			background-color: #fff
			display: block
		&:hover:after
			width: 100%
		&:not(:first-child)
			margin-left: 40px
form
	& input
		background: none
		outline: none
		border: none
		border-bottom: 1px solid $white
.pageTitle
	text-align: left
	margin-top: 180px
	padding-bottom: 200px
.title h1
	font-size: 64px
	color: $white
	font-weight: 300

.learn_link
  color: $white
  font-size: 18px
  margin-top: 24px

  text-decoration: none
  &:hover
    text-decoration: underline


.search-button
  background: none
  outline: none
  border: none
  cursor: pointer
  & .material-icons
    color: $white

#search
  color: $white
  font-size: inherit

</style>
