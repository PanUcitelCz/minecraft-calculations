<script>
	import test from '../../lib/utils/test';
	test();

	$: innerWidth = 0;
	$: innerHeight = 0;
	$: outerWidth = 0;
	$: outerHeight = 0;
	$: scrollX = 0;
	$: scrollY = 0;
	$: devicePixelRatio = 0;
</script>

<svelte:window
	bind:innerWidth
	bind:innerHeight
	bind:outerWidth
	bind:outerHeight
	bind:scrollX
	bind:scrollY
	bind:devicePixelRatio
/>
<p>innerWidth: {innerWidth}</p>
<p>innerHeight: {innerHeight}</p>
<p>outerWidth: {outerWidth}</p>
<p>outerHeight: {outerHeight}</p>
<p>scrollX: {scrollX}</p>
<p>scrollY: {scrollY}</p>
<p>devicePixelRatio: {devicePixelRatio}</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p>
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
<p style="min-width: 2000px;">
	Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae eum vitae tempora nam
	molestiae aliquam, ad excepturi omnis pariatur aperiam tenetur commodi nemo sit. Recusandae dolor
	rerum veniam a iusto.
</p>
