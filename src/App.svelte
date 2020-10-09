<script>
  import * as S from "svelte-materialify/src";
</script>

<style>
  h3 {
    margin-top: 24px;
    margin-bottom: 16px;
  }
</style>

<S.MaterialApp>
  <S.AppBar dense>
    <span slot="title"> Title </span>
    <div style="flex-grow:1;" />
    <S.Button text>Link</S.Button>
    <a href="https://github.com/TheComputerM/svelte-materialify/stargazers">
      <S.Button text>Star</S.Button>
    </a>
  </S.AppBar>
  <S.Container class="text-center">
    <h1 class="mt-4 mb-4">svelte-materialify</h1>
    <S.Divider />
  </S.Container>
  <div class="pa-4">
    <h2 class="mb-6">Some Components</h2>
    <S.Divider />
    <h3>Buttons</h3>
    <S.Button>Default</S.Button>
    <S.Button class="primary-color">Color</S.Button>
    <S.Button text>Text</S.Button>
    <S.Button outlined>Outlined</S.Button>
    <S.Badge class="primary-color" offsetX={12} offsetY={12}>
      <S.Button>Badge</S.Button>
      <span slot="badge"> 3 </span>
    </S.Badge>
    <h3>Forms</h3>
	<S.TextField>Text Field</S.TextField>
	<S.Select
      items={[{ name: 'Foo', value: 'foo' }, { name: 'Bar', value: 'bar' }, { name: 'Fizz', value: 'fizz' }, { name: 'Buzz', value: 'buzz' }]}>
      Select
    </S.Select>
    <S.Textarea>Textarea</S.Textarea>
	<S.Checkbox class="mt-2 mb-2">Checkbox</S.Checkbox>
	<S.Switch class="mt-2 mb-2">Switch</S.Switch>
    <S.Radio class="mt-2 mb-2">Radio</S.Radio>
    <S.Slider class="mt-2 mb-2">Slider</S.Slider>
  </div>
</S.MaterialApp>
