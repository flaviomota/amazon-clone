<template>
	<Head title="Address" />

	<AuthenticatedLayout>
		<div class="mt-8"></div>

		<div class="w-[500px] mx-auto text-2xl font-extrabold">
			<div>Add a new address</div>

			<form>
				<div class="text-[15px] -mb-1.5 font-extrabold">Country</div>
				<select
					class="
						w-full
						border-gray-300
						rounded-lg
						shadow-md
						py-1
						bg-gray-200
						hover:bg-gray-300
						cursor-pointer
						focus:border-orange-400
						focus:ring-orange-400
					" 
					name="country"
				>
					<option selected value="United Kingdom">United Kingdom</option>
					<option value="United Kingdom">United States</option>
					<option value="United Kingdom">Germany</option>
					<option value="United Kingdom">France</option>
					<option value="United Kingdom">Portugal</option>
				</select>

				<div class="mt-4">
					<InputLabel class="-mb-1.5" value="First name" />

					<TextInput
						class="mt-1 block w-full"
						required
						type="text"
					/>
				</div>

				<div class="mt-3">
					<InputLabel class="-mb-1.5" value="Last name" />

					<TextInput
						class="mt-1 block w-full"
						required
						type="text"
					/>
				</div>

				<div class="mt-3">
					<InputLabel class="-mb-1.5" value="Address" />

					<TextInput
						class="mt-1 block w-full"
						required
						type="text"
						placeholder="Address line 1"
					/>

					<TextInput
						class="mt-1 block w-full"
						required
						type="text"
						placeholder="Address line 2"
					/>
				</div>

				<div class="mt-3">
					<div class="flex gap-2">
						<div class="w-full">
							<InputLabel class="-mb-1.5" value="City" />

							<TextInput
								class="mt-1 block w-full"
								required
								type="text"
								placeholder="City"
							/>
						</div>

						<div class="w-full">
							<InputLabel class="-mb-1.5" value="Postcode" />

							<TextInput
								class="mt-1 block w-full"
								required
								type="text"
								placeholder="Postcode"
							/>
						</div>
					</div>
				</div>

				<div class="mt-6">
					<button class="bg-yellow-400 px-3 font-bold text-[14px] rounded-lg shadow-sm cursor-pointer">
						Add address
					</button>
				</div>
			</form>
		</div>
	</AuthenticatedLayout>
</template>

<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head, Link } from '@inertiajs/vue3';
import { toRefs } from 'vue';
import MapMarkerOutlineIcon from 'vue-material-design-icons/MapMarkerOutline.vue';
import PlusIcon from 'vue-material-design-icons/Plus.vue';
import InputLabel from '@/Components/InputLabel.vue';
import TextInput from '@/Components/TextInput.vue';

</script>

<style lang="scss" scoped>

</style>