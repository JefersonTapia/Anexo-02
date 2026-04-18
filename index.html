<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SCAT - Análisis Sistemático de Causas</title>

    <!-- Bootstrap CSS - VERSIÓN CORREGIDA -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

    <!-- SignaturePad -->
    <script src="https://cdn.jsdelivr.net/npm/signature_pad@4.1.7/dist/signature_pad.umd.min.js"></script>

    <!-- jsPDF + AutoTable -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf-autotable/3.8.4/jspdf.plugin.autotable.min.js"></script>
    
    <!-- html2canvas -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>

    <!-- FONT AWESOME CORREGIDO -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

    <style>
        :root {
            --primary-color: #1e3c72;
            --secondary-color: #2a5298;
            --accent-color: #e67e22;
            --scat-red: #c0392b;
            --scat-blue: #2980b9;
        }

        body {
            background-color: #f0f2f5;
            font-family: 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
            padding-bottom: 2rem;
        }
        
        /* Header SCAT */
        .scat-header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 1.8rem 0;
            margin-bottom: 2rem;
            border-bottom: 4px solid var(--accent-color);
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        }
        
        .scat-header h1 {
            font-weight: 600;
            font-size: 2.5rem;
            margin-bottom: 0.3rem;
            letter-spacing: 1px;
        }
        
        .scat-header h1 span {
            color: var(--accent-color);
            font-weight: 800;
        }
        
        .scat-header p {
            opacity: 0.9;
            font-size: 1.1rem;
            margin-bottom: 0;
        }
        
        .centrado {
            text-align: center;
        }
        
        .encabezado-pequeño {
            font-size: 16px;
        }
        
        .grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 8px;
        }
        
        select.form-select {
            height: auto;
            padding-right: 30px;
            white-space: normal !important;
            line-height: 1.2;
            border: 2px solid #e0e5ec;
            border-radius: 10px;
        }
        
        select.form-select:focus {
            border-color: var(--scat-blue);
            box-shadow: 0 0 0 0.2rem rgba(41, 128, 185, 0.25);
        }
        
        /* Estilo para los encabezados de sección SCAT */
        .section-header {
            background: linear-gradient(135deg, #2c3e50, #34495e);
            color: white;
            padding: 12px 20px;
            margin: 25px 0 15px 0;
            border-radius: 8px;
            font-weight: 700;
            font-size: 1.2rem;
            letter-spacing: 0.5px;
            border-left: 6px solid var(--accent-color);
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }
        
        .section-header i {
            margin-right: 10px;
            color: var(--accent-color);
        }
        
        .signature-container {
            border: 2px dashed var(--scat-blue);
            border-radius: 8px;
            padding: 10px;
            background-color: white;
            margin-top: 10px;
        }
        
        .signature-canvas {
            width: 100%;
            height: 150px;
            background-color: #fff;
            border: 1px solid #ced4da;
            border-radius: 4px;
            touch-action: none;
        }
        
        .btn-pdf {
            background: linear-gradient(135deg, #c0392b, #e74c3c);
            color: white;
            border: none;
            padding: 14px 35px;
            font-size: 1.2rem;
            font-weight: 600;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s;
            margin: 20px 0;
            box-shadow: 0 8px 20px rgba(192, 57, 43, 0.3);
            letter-spacing: 1px;
            border: 2px solid rgba(255,255,255,0.2);
        }
        
        .btn-pdf:hover {
            background: linear-gradient(135deg, #a8231a, #c0392b);
            transform: translateY(-3px);
            box-shadow: 0 12px 28px rgba(192, 57, 43, 0.4);
        }
        
        .btn-limpiar {
            background-color: #7f8c8d;
            color: white;
            border: none;
            padding: 8px 18px;
            border-radius: 25px;
            cursor: pointer;
            font-weight: 500;
            transition: all 0.3s;
        }
        
        .btn-limpiar:hover {
            background-color: #6c7a7d;
            transform: translateY(-2px);
        }
        
        .firma-label {
            font-weight: 700;
            margin-top: 15px;
            margin-bottom: 5px;
            color: var(--primary-color);
            font-size: 1.1rem;
        }
        
        /* Estilo para la tarjeta de información */
        .info-header {
            background: white;
            padding: 20px;
            border-radius: 15px;
            margin-bottom: 25px;
            border-left: 8px solid var(--accent-color);
            box-shadow: 0 8px 20px rgba(0,0,0,0.05);
            border: 1px solid #e0e5ec;
        }
        
        .info-header h5 {
            color: var(--primary-color);
            font-weight: 700;
            font-size: 1.3rem;
        }
        
        /* Grid para checkboxes */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 8px;
            background: #f8fafc;
            padding: 15px;
            border-radius: 12px;
            border: 1px solid #e0e5ec;
        }
        
        .item {
            background: white;
            padding: 6px 10px;
            border-radius: 25px;
            border: 1px solid #d0d7de;
            transition: all 0.2s;
            font-size: 0.9rem;
        }
        
        .item:hover {
            background: #e1f0fa;
            border-color: var(--scat-blue);
        }
        
        .item input[type="checkbox"] {
            margin-right: 5px;
            accent-color: var(--scat-blue);
        }
        
        /* Badge para SCAT */
        .scat-badge {
            background: var(--accent-color);
            color: white;
            padding: 5px 15px;
            border-radius: 25px;
            font-size: 0.9rem;
            font-weight: 600;
            display: inline-block;
            margin-bottom: 10px;
        }
        
        /* Footer */
        .scat-footer {
            background: white;
            padding: 15px 25px;
            border-radius: 50px;
            margin-top: 30px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.05);
            text-align: center;
            color: #6c7a89;
            font-weight: 500;
            border: 1px solid #e0e5ec;
        }
        
        .scat-footer i {
            color: var(--accent-color);
            margin: 0 5px;
        }
        
        @media (max-width: 768px) {
            .grid {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .scat-header h1 {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>

    <!-- Header SCAT -->
    <div class="scat-header">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-md-8">
                    <h1><span>Anexo 2</span> | Basic Root Cause Analysis Guide</h1>
                    <p><i class="fas fa-shield-alt me-2"></i>Guía básica para el análisis de la causa raíz</p>
                </div>
                <div class="col-md-4 text-end">
                    <div class="scat-badge">
                        <i class="fas fa-clipboard-check me-2"></i>v2.0
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="container mt-4">
        <!-- Título interno -->
        <div class="text-center mb-4">
            <hr class="w-50 mx-auto">
        </div>

        <!-- SECCIÓN: Información del Reporte -->
        <div class="info-header">
            <h5 class="fw-bold mb-3"><i class="fas fa-clipboard-list me-2" style="color: var(--accent-color);"></i>INFORMACIÓN DEL REPORTE</h5>
            <div class="row g-3">
                <div class="col-md-3">
                    <label class="fw-bold">Fecha:</label>
                    <input type="date" class="form-control" id="fechaReporte" value="2025-04-11">
                </div>
                <div class="col-md-3">
                    <label class="fw-bold">Área:</label>
                    <input type="text" class="form-control" id="area" placeholder="Ej: Operaciones, Mina">
                </div>
                <div class="col-md-3">
                    <label class="fw-bold">Supervisor:</label>
                    <input type="text" class="form-control" id="supervisor" placeholder="Nombre del supervisor">
                </div>
                <div class="col-md-3">
                    <label class="fw-bold">Unidad Minera:</label>
                    <select class="form-select" id="unidadMinera">
                        <option value="">-- Seleccione --</option>
                        <option value="Cerro Verde">Cerro Verde</option>
                        <option value="AngloAmerican">AngloAmerican</option>
                        <option value="HUDBAY">HUDBAY</option>
                        <option value="Marcobre">Marcobre</option>
                        <option value="Southern">Southern</option>
                        <option value="Antamina">Antamina</option>
                        <option value="Yanacocha">Yanacocha</option>
                    </select>
                </div>
            </div>
        </div>
        <!-- SECCIÓN 1: LESIONES - PARTES DEL CUERPO -->
        <div class="section-header">
            <i class="fas fa-user-injured"></i>1. PARTES DEL CUERPO AFECTADAS
        </div>
        <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 5px;">
            <div><input type="checkbox" id="i1" value="Cabeza"> <label for="i1">1.1 Cabeza</label></div>
            <div><input type="checkbox" id="i2" value="Ojo"> <label for="i2">1.2 Ojo</label></div>
            <div><input type="checkbox" id="i3" value="Nariz"> <label for="i3">1.3 Nariz</label></div>
            <div><input type="checkbox" id="i4" value="Diente(s)"> <label for="i4">1.4 Diente(s)</label></div>
            <div><input type="checkbox" id="i5" value="Mandíbula"> <label for="i5">1.5 Mandíbula</label></div>
            <div><input type="checkbox" id="i6" value="Cara"> <label for="i6">1.6 Cara</label></div>
            <div><input type="checkbox" id="i7" value="Oído"> <label for="i7">1.7 Oído</label></div>
            <div><input type="checkbox" id="i8" value="Cuello"> <label for="i8">1.8 Cuello</label></div>
            <div><input type="checkbox" id="i9" value="Hombro"> <label for="i9">1.9 Hombro</label></div>
            <div><input type="checkbox" id="i10" value="Brazo superior"> <label for="i10">1.10 Brazo superior</label></div>
            <div><input type="checkbox" id="i11" value="Codo"> <label for="i11">1.11 Codo</label></div>
            <div><input type="checkbox" id="i12" value="Antebrazo"> <label for="i12">1.12 Antebrazo</label></div>
            <div><input type="checkbox" id="i13" value="Muñeca"> <label for="i13">1.13 Muñeca</label></div>
            <div><input type="checkbox" id="i14" value="Mano"> <label for="i14">1.14 Mano</label></div>
            <div><input type="checkbox" id="i15" value="Dedo"> <label for="i15">1.15 Dedo</label></div>
            <div><input type="checkbox" id="i16" value="Pecho"> <label for="i16">1.16 Pecho</label></div>
            <div><input type="checkbox" id="i17" value="Abdomen"> <label for="i17">1.17 Abdomen</label></div>
            <div><input type="checkbox" id="i18" value="Columna Dorsal"> <label for="i18">1.18 Columna Dorsal</label></div>
            <div><input type="checkbox" id="i19" value="Columna Lumbar"> <label for="i19">1.19 Columna Lumbar</label></div>
            <div><input type="checkbox" id="i20" value="Caderas"> <label for="i20">1.20 Caderas</label></div>
            <div><input type="checkbox" id="i21" value="Nalgas"> <label for="i21">1.21 Nalgas</label></div>
            <div><input type="checkbox" id="i22" value="Ingle"> <label for="i22">1.22 Ingle</label></div>
            <div><input type="checkbox" id="i23" value="Pierna superior"> <label for="i23">1.23 Pierna superior</label></div>
            <div><input type="checkbox" id="i24" value="Rodilla"> <label for="i24">1.24 Rodilla</label></div>
            <div><input type="checkbox" id="i25" value="Pierna Inferior"> <label for="i25">1.25 Pierna Inferior</label></div>
            <div><input type="checkbox" id="i26" value="Tobillo"> <label for="i26">1.26 Tobillo</label></div>
            <div><input type="checkbox" id="i27" value="Pié"> <label for="i27">1.27 Pié</label></div>
            <div><input type="checkbox" id="i28" value="Dedo del Pié"> <label for="i28">1.28 Dedo del Pié</label></div>
            <div><input type="checkbox" id="i29" value="Interno"> <label for="i29">1.29 Interno</label></div>
            <div><input type="checkbox" id="i30" value="Sistémico"> <label for="i30">1.30 Sistémico</label></div>
        </div>

        <!-- SECCIÓN 2: NATURALEZA DE LA LESIÓN -->
        <div class="section-header">
            <i class="fas fa-notes-medical"></i>2. NATURALEZA DE LA LESIÓN
        </div>

        <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 5px;">
            <div><input type="checkbox" id="i31" value="Abrasión"> <label for="i31">2.1 Abrasión</label></div>
            <div><input type="checkbox" id="i32" value="Alergia"> <label for="i32">2.2 Alergia</label></div>
            <div><input type="checkbox" id="i33" value="Amputación"> <label for="i33">2.3 Amputación</label></div>
            <div><input type="checkbox" id="i34" value="Mordida/Picada"> <label for="i34">2.4 Mordida/Picada</label></div>
            <div><input type="checkbox" id="i35" value="Moretón/Contusión"> <label for="i35">2.5 Moretón/Contusión</label></div>
            <div><input type="checkbox" id="i36" value="Quemadura química"> <label for="i36">2.6 Quemadura (química)</label></div>
            <div><input type="checkbox" id="i37" value="Quemadura eléctrica"> <label for="i37">2.7 Quemadura (eléctrica)</label></div>
            <div><input type="checkbox" id="i38" value="Quemadura calor"> <label for="i38">2.8 Quemadura (calor)</label></div>
            <div><input type="checkbox" id="i39" value="Conmoción Cerebral"> <label for="i39">2.9 Conmoción Cerebral</label></div>
            <div><input type="checkbox" id="i40" value="Corte/Esquina"> <label for="i40">2.10 Corte/Esquina</label></div>
            <div><input type="checkbox" id="i41" value="Aplastamiento"> <label for="i41">2.11 Aplastamiento</label></div>
            <div><input type="checkbox" id="i42" value="Corte/Laceración"> <label for="i42">2.12 Corte/Laceración</label></div>
            <div><input type="checkbox" id="i43" value="Dislocación"> <label for="i43">2.13 Dislocación</label></div>
            <div><input type="checkbox" id="i44" value="Agotamiento"> <label for="i44">2.14 Agotamiento</label></div>
            <div><input type="checkbox" id="i45" value="Intoxicación Alimentaria"> <label for="i45">2.15 Intoxicación por Alimento</label></div>
            <div><input type="checkbox" id="i46" value="Cuerpo Extraño Incrustado"> <label for="i46">2.16 Cuerpo Extraño [incrustado]</label></div>
            <div><input type="checkbox" id="i47" value="Cuerpo Extraño Liberado"> <label for="i47">2.17 Cuerpo Extraño [liberado]</label></div>
            <div><input type="checkbox" id="i48" value="Fractura"> <label for="i48">2.18 Fractura</label></div>
            <div><input type="checkbox" id="i49" value="Dolor de Cabeza"> <label for="i49">2.19 Dolor de Cabeza</label></div>
            <div><input type="checkbox" id="i50" value="Hernia"> <label for="i50">2.20 Hernia</label></div>
            <div><input type="checkbox" id="i51" value="Hipotermia"> <label for="i51">2.21 Hipotermia</label></div>
            <div><input type="checkbox" id="i52" value="Inhalación"> <label for="i52">2.22 Inhalación</label></div>
            <div><input type="checkbox" id="i53" value="Irritación"> <label for="i53">2.23 Irritación</label></div>
            <div><input type="checkbox" id="i54" value="Obstrucción"> <label for="i54">2.24 Obstrucción</label></div>
            <div><input type="checkbox" id="i55" value="Envenenamiento"> <label for="i55">2.25 Envenenamiento</label></div>
            <div><input type="checkbox" id="i56" value="Pinchazo"> <label for="i56">2.26 Pinchazo</label></div>
            <div><input type="checkbox" id="i57" value="Shock"> <label for="i57">2.27 Shock</label></div>
            <div><input type="checkbox" id="i58" value="Esguince/Tensión"> <label for="i58">2.28 Esguince/Tensión</label></div>
            <div><input type="checkbox" id="i59" value="Asfixia"> <label for="i59">2.29 Asfixia</label></div>
            <div><input type="checkbox" id="i60" value="Herida"> <label for="i60">2.30 Herida</label></div>
        </div>

        <!-- SECCIÓN 3: CONTACTO - AGENCIA Y MECANISMO -->
        <div class="section-header">
            <i class="fas fa-bolt"></i>3. CONTACTO - AGENCIA Y MECANISMO
        </div>
        <div class="row g-3 mb-3">
            <div class="col-md-6">
                <label class="fw-bold">AGENCIA INVOLUCRADA (única)</label>
                <select class="form-select" id="agencia" name="agencia">
                    <option value="">-- Seleccione Agencia --</option>
                    <option value="3.1 Avión/Barco">3.1 Avión/Barco</option>
                    <option value="3.2 Animal/Fauna">3.2 Animal/Fauna</option>
                    <option value="3.3 Caldera">3.3 Caldera</option>
                    <option value="3.4 Construcción">3.4 Construcción</option>
                    <option value="3.5 Químicos">3.5 Químicos</option>
                    <option value="3.6 Contenedores">3.6 Contenedores</option>
                    <option value="3.7 Transportadoras">3.7 Transportadoras</option>
                    <option value="3.8 Polvo">3.8 Polvo</option>
                    <option value="3.9 Aparatos Eléctricos">3.9 Aparatos Eléctricos</option>
                    <option value="3.10 Ascensor">3.10 Ascensor</option>
                    <option value="3.11 Explosivo">3.11 Explosivo</option>
                    <option value="3.12 Pasarela">3.12 Pasarela</option>
                    <option value="3.13 Gases">3.13 Gases</option>
                    <option value="3.14 Herramientas Manuales">3.14 Herramientas Manuales</option>
                    <option value="3.15 Equipo Pesado">3.15 Equipo Pesado</option>
                    <option value="3.16 Calor/Inflamable">3.16 Calor/Inflamable</option>
                    <option value="3.17 Aparatos de Izaje">3.17 Aparatos de Izaje</option>
                    <option value="3.18 Instalación">3.18 Instalación</option>
                    <option value="3.19 Escaleras">3.19 Escaleras</option>
                    <option value="3.20 Vehículo Liviano">3.20 Vehículo Liviano</option>
                    <option value="3.21 Maquinaria">3.21 Maquinaria</option>
                    <option value="3.22 Material/Bienes">3.22 Material/Bienes</option>
                    <option value="3.23 Transmisión Mecánica">3.23 Transmisión Mecánica</option>
                    <option value="3.24 Obstrucción">3.24 Obstrucción</option>
                    <option value="3.25 Proyectil">3.25 Proyectil</option>
                    <option value="3.26 Radiación">3.26 Radiación</option>
                    <option value="3.27 Borde Cortante">3.27 Borde Cortante</option>
                    <option value="3.28 Tensión Suelo">3.28 Tensión Suelo</option>
                    <option value="3.29 Trabajos Superficie">3.29 Trabajos Superficie</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">MECANISMO DE LESIÓN (única)</label>
                <select class="form-select" id="mecanismo" name="mecanismo">
                    <option value="">-- Seleccione Mecanismo --</option>
                    <option value="4.1 Agravante">4.1 Agravante</option>
                    <option value="4.2 Mordedura/Picadura">4.2 Mordedura/Picadura</option>
                    <option value="4.3 Explosión">4.3 Explosión</option>
                    <option value="4.4 Reacción Física">4.4 Reacción Física</option>
                    <option value="4.5 Alcanzado (Pellizco)">4.5 Alcanzado</option>
                    <option value="4.6 Agarrado">4.6 Agarrado</option>
                    <option value="4.7 Atrapado">4.7 Atrapado</option>
                    <option value="4.8 Contacto con">4.8 Contacto con</option>
                    <option value="4.9 Exposición temperaturas">4.9 Exposición temperaturas</option>
                    <option value="4.10 Caída desde altura">4.10 Caída desde altura</option>
                    <option value="4.11 Caída mismo nivel">4.11 Caída mismo nivel</option>
                    <option value="4.12 Cuerpo extraño en ojo">4.12 Cuerpo extraño en ojo</option>
                    <option value="4.13 Inhalación">4.13 Inhalación</option>
                    <option value="4.14 Levantar/Tirar/Empujar">4.14 Levantar/Tirar/Empujar</option>
                    <option value="4.15 Sobre esfuerzo">4.15 Sobre esfuerzo</option>
                    <option value="4.16 Roce/Desgaste">4.16 Roce/Desgaste</option>
                    <option value="4.17 Descarga Eléctrica">4.17 Descarga Eléctrica</option>
                    <option value="4.18 Resbalón">4.18 Resbalón</option>
                    <option value="4.19 Golpear contra">4.19 Golpear contra</option>
                    <option value="4.20 Alcanzado por objeto">4.20 Alcanzado por objeto</option>
                </select>
            </div>
        </div>

        <!-- SECCIÓN 4: CAUSAS INMEDIATAS -->
        <div class="section-header">
            <i class="fas fa-exclamation-triangle"></i>4. CAUSAS INMEDIATAS
        </div>
        <div class="row g-3 mb-3">
            <div class="col-md-6">
                <label class="fw-bold">PRÁCTICAS SUB-ESTÁNDAR (única)</label>
                <select class="form-select" id="practica" name="practica">
                    <option value="">-- Seleccione Práctica --</option>
                    <option value="5.1 Falla en seguir procedimiento">5.1 Falla en seguir procedimiento</option>
                    <option value="5.2 Inspección inadecuada">5.2 Inspección inadecuada</option>
                    <option value="5.3 Inspección pre-operativa inadecuada">5.3 Inspección pre-operativa inadecuada</option>
                    <option value="5.4 Evaluación riesgo incorrecta">5.4 Evaluación riesgo incorrecta</option>
                    <option value="5.5 No iniciar acción correctiva">5.5 No iniciar acción correctiva</option>
                    <option value="5.6 Proceder sin autoridad">5.6 Proceder sin autoridad</option>
                    <option value="5.7 Falla en alertar">5.7 Falla en alertar</option>
                    <option value="5.8 Falla de seguridad">5.8 Falla de seguridad</option>
                    <option value="5.9 Velocidad inapropiada">5.9 Velocidad inapropiada</option>
                    <option value="5.10 Quitar elementos seguridad">5.10 Quitar elementos seguridad</option>
                    <option value="5.11 Equipo defectuoso">5.11 Equipo defectuoso</option>
                    <option value="5.12 Uso inapropiado equipo">5.12 Uso inapropiado equipo</option>
                    <option value="5.13 Defecto en uso EPP">5.13 Defecto en uso EPP</option>
                    <option value="5.14 Carga incorrecta">5.14 Carga incorrecta</option>
                    <option value="5.15 Ubicación incorrecta">5.15 Ubicación incorrecta</option>
                    <option value="5.16 Levantar indebidamente">5.16 Levantar indebidamente</option>
                    <option value="5.17 Posición inadecuada">5.17 Posición inadecuada</option>
                    <option value="5.18 Acción temeraria">5.18 Acción temeraria</option>
                    <option value="5.19 Alcohol/drogas">5.19 Alcohol/drogas</option>
                    <option value="5.20 Incapacitado">5.20 Incapacitado</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">CONDICIONES SUB-ESTÁNDAR (única)</label>
                <select class="form-select" id="condicion" name="condicion">
                    <option value="">-- Seleccione Condición --</option>
                    <option value="6.1 Guardias inadecuadas">6.1 Guardias inadecuadas</option>
                    <option value="6.2 EPP inadecuado">6.2 EPP inadecuado</option>
                    <option value="6.3 Equipos defectuosos">6.3 Equipos defectuosos</option>
                    <option value="6.4 Congestión">6.4 Congestión</option>
                    <option value="6.5 Sistema advertencia inadecuado">6.5 Sistema advertencia inadecuado</option>
                    <option value="6.6 Incendio/Explosión">6.6 Incendio/Explosión</option>
                    <option value="6.7 Falta aseo">6.7 Falta aseo</option>
                    <option value="6.8 Condiciones ambientales peligrosas">6.8 Condiciones ambientales</option>
                    <option value="6.9 Exposición ruido">6.9 Exposición ruido</option>
                    <option value="6.10 Exposición radiación">6.10 Exposición radiación</option>
                    <option value="6.11 Temperaturas extremas">6.11 Temperaturas extremas</option>
                    <option value="6.12 Iluminación inadecuada">6.12 Iluminación inadecuada</option>
                    <option value="6.13 Ventilación inadecuada">6.13 Ventilación inadecuada</option>
                </select>
            </div>
        </div>

        <!-- SECCIÓN 5: FACTOR PERSONAL -->
        <div class="section-header">
            <i class="fas fa-user"></i>5. FACTOR PERSONAL (SCAT)
        </div>
        <div class="row g-3 mb-3">
            <div class="col-md-6">
                <label class="fw-bold">OPCIÓN 1</label>
                <select class="form-select" id="opcionfp1">
                    <option value="">-- Seleccione Factor Personal --</option>
                    <option value="FP-01">7.1 CAPACIDAD FÍSICA INADECUADA</option>
                    <option value="FP-02">7.2 CAPACIDAD MENTAL DEFICIENTE</option>
                    <option value="FP-03">7.3 ESTRÉS FÍSICO</option>
                    <option value="FP-04">7.4 ESTRÉS MENTAL</option>
                    <option value="FP-05">7.5 FALTA DE CONOCIMIENTO</option>
                    <option value="FP-06">7.6 FALTA DE APTITUDES</option>
                    <option value="FP-07">7.7 MOTIVACIÓN INCORRECTA</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">SUBGRUPO 1</label>
                <select class="form-select" id="subgrupofp1">
                    <option value="">-- Seleccione subgrupo --</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">OPCIÓN 2 (opcional)</label>
                <select class="form-select" id="opcionfp2">
                    <option value="">-- Seleccione Factor Personal --</option>
                    <option value="FP-01">7.1 CAPACIDAD FÍSICA INADECUADA</option>
                    <option value="FP-02">7.2 CAPACIDAD MENTAL DEFICIENTE</option>
                    <option value="FP-03">7.3 ESTRÉS FÍSICO</option>
                    <option value="FP-04">7.4 ESTRÉS MENTAL</option>
                    <option value="FP-05">7.5 FALTA DE CONOCIMIENTO</option>
                    <option value="FP-06">7.6 FALTA DE APTITUDES</option>
                    <option value="FP-07">7.7 MOTIVACIÓN INCORRECTA</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">SUBGRUPO 2</label>
                <select class="form-select" id="subgrupofp2">
                    <option value="">-- Seleccione subgrupo --</option>
                </select>
            </div>
        </div>

        <!-- SECCIÓN 6: FACTOR DE TRABAJO -->
        <div class="section-header">
            <i class="fas fa-hard-hat"></i>6. FACTOR DE TRABAJO (SCAT)
        </div>
        <div class="row g-3 mb-3">
            <div class="col-md-6">
                <label class="fw-bold">OPCIÓN 1</label>
                <select class="form-select" id="opcion1">
                    <option value="">-- Seleccione Factor Trabajo --</option>
                    <option value="FT-01">8.1 LIDERAZGO INADECUADO</option>
                    <option value="FT-02">8.2 INGENIERÍA INADECUADA</option>
                    <option value="FT-03">8.3 COMPRAS INCORRECTAS</option>
                    <option value="FT-04">8.4 MANTENCIÓN INADECUADA</option>
                    <option value="FT-05">8.5 HERRAMIENTAS INADECUADAS</option>
                    <option value="FT-06">8.6 ESTÁNDARES INADECUADOS</option>
                    <option value="FT-07">8.7 DESGASTE</option>
                    <option value="FT-08">8.8 ABUSO/MAL USO</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">SUBGRUPO 1</label>
                <select class="form-select" id="subgrupo1">
                    <option value="">-- Seleccione subgrupo --</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">OPCIÓN 2 (opcional)</label>
                <select class="form-select" id="opcion2">
                    <option value="">-- Seleccione Factor Trabajo --</option>
                    <option value="FT-01">8.1 LIDERAZGO INADECUADO</option>
                    <option value="FT-02">8.2 INGENIERÍA INADECUADA</option>
                    <option value="FT-03">8.3 COMPRAS INCORRECTAS</option>
                    <option value="FT-04">8.4 MANTENCIÓN INADECUADA</option>
                    <option value="FT-05">8.5 HERRAMIENTAS INADECUADAS</option>
                    <option value="FT-06">8.6 ESTÁNDARES INADECUADOS</option>
                    <option value="FT-07">8.7 DESGASTE</option>
                    <option value="FT-08">8.8 ABUSO/MAL USO</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">SUBGRUPO 2</label>
                <select class="form-select" id="subgrupo2">
                    <option value="">-- Seleccione subgrupo --</option>
                </select>
            </div>
        </div>

        <!-- SECCIÓN 7: CONTROL DE GERENCIA -->
        <div class="section-header">
            <i class="fas fa-chart-line"></i>7. CONTROL DE GERENCIA
        </div>
        <div class="row g-3 mb-3">
            <div class="col-md-6">
                <label class="fw-bold">OPCIÓN 1</label>
                <select class="form-select" id="opcioncg1">
                    <option value="">-- Seleccione Control --</option>
                    <option value="CG-01">9.1 DESARROLLO DEL EMPLEADO</option>
                    <option value="CG-02">9.2 ACCOUNTABILITY</option>
                    <option value="CG-03">9.3 MANEJO DE RIESGO/CAMBIO</option>
                    <option value="CG-04">9.4 COMUNICACIONES</option>
                    <option value="CG-05">9.5 INSPECCIONES/AUDITORÍAS</option>
                    <option value="CG-06">9.6 PREPARACIÓN EMERGENCIAS</option>
                    <option value="CG-07">9.7 POLÍTICAS/INSTRUCCIONES</option>
                    <option value="CG-08">9.8 MANEJO CONTRATISTAS</option>
                    <option value="CG-09">9.9 INGENIERÍA/DISEÑO</option>
                    <option value="CG-10">9.10 OPERACIONES/MANTENCIÓN</option>
                    <option value="CG-11">9.11 SALUD OCUPACIONAL</option>
                    <option value="CG-12">9.12 ERGONOMÍA</option>
                    <option value="CG-13">9.13 RECURSOS HUMANOS</option>
                    <option value="CG-14">9.14 MEDIOAMBIENTE</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">SUBGRUPO 1</label>
                <select class="form-select" id="subgrupocg1">
                    <option value="">-- Seleccione subgrupo --</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">OPCIÓN 2 (opcional)</label>
                <select class="form-select" id="opcioncg2">
                    <option value="">-- Seleccione Control --</option>
                    <option value="CG-01">9.1 DESARROLLO DEL EMPLEADO</option>
                    <option value="CG-02">9.2 ACCOUNTABILITY</option>
                    <option value="CG-03">9.3 MANEJO DE RIESGO/CAMBIO</option>
                    <option value="CG-04">9.4 COMUNICACIONES</option>
                    <option value="CG-05">9.5 INSPECCIONES/AUDITORÍAS</option>
                    <option value="CG-06">6.6 PREPARACIÓN EMERGENCIAS</option>
                    <option value="CG-07">9.7 POLÍTICAS/INSTRUCCIONES</option>
                    <option value="CG-08">9.8 MANEJO CONTRATISTAS</option>
                    <option value="CG-09">9.9 INGENIERÍA/DISEÑO</option>
                    <option value="CG-10">9.10 OPERACIONES/MANTENCIÓN</option>
                    <option value="CG-11">9.11 SALUD OCUPACIONAL</option>
                    <option value="CG-12">9.12 ERGONOMÍA</option>
                    <option value="CG-13">9.13 RECURSOS HUMANOS</option>
                    <option value="CG-14">9.14 MEDIOAMBIENTE</option>
                </select>
            </div>
            <div class="col-md-6">
                <label class="fw-bold">SUBGRUPO 2</label>
                <select class="form-select" id="subgrupocg2">
                    <option value="">-- Seleccione subgrupo --</option>
                </select>
            </div>
        </div>

        <!-- SECCIÓN 8: FIRMAS -->
        <div class="section-header">
            <i class="fas fa-signature"></i>8. FIRMAS
        </div>
        <div class="row">
            <div class="col-md-6 mb-4">
                <div class="firma-label">Firma del Investigador:</div>
                <div class="signature-container">
                    <canvas id="signature1" class="signature-canvas"></canvas>
                </div>
                <button class="btn-limpiar mt-2" onclick="limpiarFirma(1)">Limpiar Firma</button>
            </div>
            <div class="col-md-6 mb-4">
                <div class="firma-label">Firma del Supervisor:</div>
                <div class="signature-container">
                    <canvas id="signature2" class="signature-canvas"></canvas>
                </div>
                <button class="btn-limpiar mt-2" onclick="limpiarFirma(2)">Limpiar Firma</button>
            </div>
        </div>

        <!-- Botón PDF -->
        <div class="text-center">
            <button class="btn-pdf" onclick="generarPDF()">
                <i class="fas fa-file-pdf me-2"></i>GENERAR REPORTE SCAT
            </button>
        </div>

        <!-- Footer -->
        <div class="scat-footer">
            <i class="fas fa-user-circle"></i> Analista: Jeferson_QT 
            <i class="fas fa-envelope mx-3"></i> jeferson7316@hotmail.com
            <i class="fas fa-code-branch"></i> SCAT v2.0
        </div>
    </div>

    <script>
        // ============================================
        // CONFIGURACIÓN DE FIRMAS
        // ============================================
        let signaturePad1, signaturePad2;

        function initSignatures() {
            const canvas1 = document.getElementById('signature1');
            const canvas2 = document.getElementById('signature2');
            
            function resizeCanvas(canvas) {
                const ratio = Math.max(window.devicePixelRatio || 1, 1);
                canvas.width = canvas.offsetWidth * ratio;
                canvas.height = canvas.offsetHeight * ratio;
                canvas.getContext("2d").scale(ratio, ratio);
            }
            
            resizeCanvas(canvas1);
            resizeCanvas(canvas2);
            
            signaturePad1 = new SignaturePad(canvas1, {
                backgroundColor: 'rgb(255, 255, 255)',
                penColor: 'rgb(0, 0, 0)'
            });
            
            signaturePad2 = new SignaturePad(canvas2, {
                backgroundColor: 'rgb(255, 255, 255)',
                penColor: 'rgb(0, 0, 0)'
            });
        }

        function limpiarFirma(num) {
            if (num === 1 && signaturePad1) signaturePad1.clear();
            if (num === 2 && signaturePad2) signaturePad2.clear();
        }

        // ============================================
        // DATOS DE SUBGRUPOS
        // ============================================
        const subgrupofpData = {
            "FP-01":["7.1.1 Altura/peso/fuerza inadecuados","7.1.2 Rango movimiento limitado","7.1.3 Capacidad posición limitada","7.1.4 Incapacidad permanente","7.1.5 Incapacidad temporal","7.1.6 Alergias","7.1.7 Sensibilidad sensorial","7.1.8 Visión deficiente","7.1.9 Audición deficiente","7.1.10 Otros sentidos","7.1.11 Incapacidad respiratoria"],
            "FP-02":["7.2.1 Discapacidad permanente","7.2.2 Discapacidad temporal","7.2.3 Miedos/Fobias","7.2.4 Alteración emocional","7.2.5 Enfermedad mental","7.2.6 Nivel inteligencia","7.2.7 Incapacidad comprensión"],
            "FP-03":["7.3.1 Lesión/enfermedad","7.3.2 Fatiga por carga","7.3.3 Fatiga por descanso","7.3.4 Sobrecarga sensorial","7.3.5 Exposición peligros"],
            "FP-04":["7.4.1 Sobrecarga emocional","7.4.2 Fatiga por presión","7.4.3 Exigencia decisiones","7.4.4 Monotonía","7.4.5 Exigencia concentración"],
            "FP-05":["7.5.1 Falta experiencia","7.5.2 Orientación inadecuada","7.5.3 Capacitación insuficiente"],
            "FP-06":["7.6.1 Instrucción insuficiente","7.6.2 Desempeño inadecuado","7.6.3 Práctica infrecuente"],
            "FP-07":["7.7.1 Premio práctica impropia","7.7.2 Castigo práctica correcta","7.7.3 Falta incentivos","7.7.4 Frustración excesiva"]
        };

        const subgrupoData = {
            "FT-01":["8.1.1 Informe poco claro","8.1.2 Responsabilidad confusa","8.1.3 Delegación inapropiada","8.1.4 Políticas inapropiadas","8.1.5 Planificación inadecuada","8.1.6 Instrucciones incorrectas"],
            "FT-02":["8.2.1 Evaluación inadecuada","8.2.2 Ergonomía inadecuada","8.2.3 Estándares inadecuados","8.2.4 Monitoreo inadecuado"],
            "FT-03":["8.3.1 Especificaciones incorrectas","8.3.2 Investigación incorrecta","8.3.3 Inspección inadecuada"],
            "FT-04":["8.4.1 Prevención inadecuada","8.4.2 Restauración inadecuada","8.4.3 Reparación inadecuada"],
            "FT-05":["8.5.1 Evaluación necesidades","8.5.2 Factores ergonómicos","8.5.3 Especificaciones inadecuadas"],
            "FT-06":["8.6.1 Desarrollo inadecuado","8.6.2 Comunicación inadecuada","8.6.3 Mantención inadecuada"],
            "FT-07":["8.7.1 Planificación uso","8.7.2 Inspección inadecuada","8.7.3 Mantención inadecuada"],
            "FT-08":["8.8.1 Tolerado por supervisión","8.8.2 No tolerado"]
        };

        const subgrupocgData = {
            "CG-01":["9.1.1 Necesidades capacitación","9.1.2 Materiales desarrollados","9.1.3 Capacitación nuevos","9.1.4 Registros"],
            "CG-02":["9.2.1 Sistema establecido","9.2.2 Roles definidos","9.2.3 Evaluaciones regulares"],
            "CG-03":["9.3.1 Riesgos identificados","9.3.2 Riesgos analizados","9.3.3 Controles identificados"],
            "CG-04":["9.4.1 Comunicación general","9.4.2 Reuniones grupo","9.4.3 Efectividad"],
            "CG-05":["9.5.1 Inspección planeada","9.5.2 Inspección lugar","9.5.3 Seguimiento"],
            "CG-06":["9.6.1 Roles establecidos","9.6.2 Planes escritos","9.6.3 Equipos"],
            "CG-07":["9.7.1 Desarrollados para tareas","9.7.2 Disponibles","9.7.3 Revisados"],
            "CG-08":["9.8.1 Políticas escritas","9.8.2 Selección contratistas","9.8.3 Capacitación"],
            "CG-09":["9.9.1 Normas seguidas","9.9.2 Peligros identificados","9.9.3 Revisión proyectos"],
            "CG-10":["9.10.1 Mantención preventiva","9.10.2 Partes críticas","9.10.3 Sistema pedidos"],
            "CG-11":["9.11.1 Evaluación peligros","9.11.2 Monitoreo","9.11.3 Supervisión médica"],
            "CG-12":["9.12.1 Diseño ergonómico","9.12.2 Revisiones","9.12.3 Capacitación"],
            "CG-13":["9.13.1 Requisitos evaluados","9.13.2 Examen precolocación","9.13.3 Inducción"],
            "CG-14":["9.14.1 Controles derrames"]
        };

        // ============================================
        // FUNCIONES PARA CARGAR SUBGRUPOS
        // ============================================
        function cargarSubgrupofp(origenSelect, destinoSelectId) {
            const valor = origenSelect.value;
            const destino = document.getElementById(destinoSelectId);
            destino.innerHTML = '<option value="">-- Seleccione subgrupo --</option>';
            
            if (subgrupofpData[valor]) {
                subgrupofpData[valor].forEach(txt => {
                    const opt = document.createElement("option");
                    opt.value = txt;
                    opt.textContent = txt;
                    destino.appendChild(opt);
                });
            }
        }

        function cargarSubgrupo(origenSelect, destinoSelectId) {
            const valor = origenSelect.value;
            const destino = document.getElementById(destinoSelectId);
            destino.innerHTML = '<option value="">-- Seleccione subgrupo --</option>';
            
            if (subgrupoData[valor]) {
                subgrupoData[valor].forEach(txt => {
                    const opt = document.createElement("option");
                    opt.value = txt;
                    opt.textContent = txt;
                    destino.appendChild(opt);
                });
            }
        }

        function cargarSubgrupocg(origenSelect, destinoSelectId) {
            const valor = origenSelect.value;
            const destino = document.getElementById(destinoSelectId);
            destino.innerHTML = '<option value="">-- Seleccione subgrupo --</option>';
            
            if (subgrupocgData[valor]) {
                subgrupocgData[valor].forEach(txt => {
                    const opt = document.createElement("option");
                    opt.value = txt;
                    opt.textContent = txt;
                    destino.appendChild(opt);
                });
            }
        }

        // ============================================
        // FUNCIÓN PRINCIPAL PARA GENERAR PDF
        // ============================================
        async function generarPDF() {
            const { jsPDF } = window.jspdf;
            const pdf = new jsPDF('p', 'pt', 'a4');
            
            const pageWidth = pdf.internal.pageSize.getWidth();
            const pageHeight = pdf.internal.pageSize.getHeight();
            const margin = 50;
            let yPos = 50;
            let pageNumber = 1;

            function checkSpace(needed) {
                if (yPos + needed > pageHeight - 50) {
                    pdf.addPage();
                    pageNumber++;
                    yPos = 50;
                    return true;
                }
                return false;
            }

            // Encabezado
            pdf.setFillColor(30, 60, 114);
            pdf.rect(0, 0, pageWidth, 60, 'F');
            pdf.setTextColor(255, 255, 255);
            pdf.setFontSize(28);
            pdf.setFont('helvetica', 'bold');
            pdf.text('ANEXO 2', margin, 40);
            pdf.setFontSize(14);
            pdf.setFont('helvetica', 'normal');
            pdf.text('Basic Root Cause Analysis Guide', margin, 55);
            
            yPos = 80;

            // Título
            checkSpace(40);
            pdf.setTextColor(30, 60, 114);
            pdf.setFontSize(18);
            pdf.setFont('helvetica', 'bold');
            pdf.text('INFORME DE ANÁLISIS CAUSA RAÍZ BÁSICO', pageWidth/2, yPos, { align: 'center' });
            yPos += 25;
            pdf.setDrawColor(200, 200, 200);
            pdf.line(margin, yPos, pageWidth - margin, yPos);
            yPos += 20;

            // Datos del reporte
            checkSpace(80);
            pdf.setFillColor(44, 62, 80);
            pdf.rect(margin, yPos-15, pageWidth - (2*margin), 25, 'F');
            pdf.setTextColor(255, 255, 255);
            pdf.setFontSize(13);
            pdf.setFont('helvetica', 'bold');
            pdf.text('INFORMACIÓN DEL REPORTE', margin + 10, yPos);
            yPos += 25;
            pdf.setTextColor(0, 0, 0);
            pdf.setFontSize(11);
            
            const fecha = document.getElementById('fechaReporte').value || 'No especificada';
            const area = document.getElementById('area').value || 'No especificada';
            const supervisor = document.getElementById('supervisor').value || 'No especificado';
            const unidad = document.getElementById('unidadMinera').value || 'No especificada';
            
            pdf.setFont('helvetica', 'bold');
            pdf.text('Fecha:', margin, yPos);
            pdf.setFont('helvetica', 'normal');
            pdf.text(fecha, margin + 55, yPos);
            pdf.setFont('helvetica', 'bold');
            pdf.text('Área:', margin + 220, yPos);
            pdf.setFont('helvetica', 'normal');
            pdf.text(area, margin + 270, yPos);
            yPos += 20;
            
            pdf.setFont('helvetica', 'bold');
            pdf.text('Supervisor:', margin, yPos);
            pdf.setFont('helvetica', 'normal');
            pdf.text(supervisor, margin + 80, yPos);
            pdf.setFont('helvetica', 'bold');
            pdf.text('Unidad Minera:', margin + 220, yPos);
            pdf.setFont('helvetica', 'normal');
            pdf.text(unidad, margin + 320, yPos);
            yPos += 30;
            pdf.line(margin, yPos, pageWidth - margin, yPos);
            yPos += 20;

            // Partes del cuerpo
            checkSpace(80);
            pdf.setFillColor(44, 62, 80);
            pdf.rect(margin, yPos-15, pageWidth - (2*margin), 25, 'F');
            pdf.setTextColor(255, 255, 255);
            pdf.text('1. PARTES DEL CUERPO AFECTADAS', margin + 10, yPos);
            yPos += 20;
            pdf.setTextColor(0, 0, 0);
            
            const partes = [];
            for (let i = 1; i <= 30; i++) {
                const chk = document.getElementById(`i${i}`);
                if (chk && chk.checked) {
                    const label = chk.nextElementSibling;
                    partes.push(label ? label.textContent.trim() : `Opción ${i}`);
                }
            }
            
            pdf.setFontSize(10);
            pdf.setFont('helvetica', 'normal');
            if (partes.length > 0) {
                const texto = partes.join(', ');
                const lineas = pdf.splitTextToSize(texto, pageWidth - (2*margin) - 30);
                if (yPos + (lineas.length * 14) > pageHeight - 60) {
                    pdf.addPage();
                    pageNumber++;
                    yPos = 50;
                }
                pdf.text(lineas, margin + 10, yPos);
                yPos += (lineas.length * 14) + 15;
            } else {
                pdf.text('Ninguna parte seleccionada', margin + 10, yPos);
                yPos += 25;
            }

            // Naturaleza de la lesión
            checkSpace(80);
            pdf.setFillColor(44, 62, 80);
            pdf.rect(margin, yPos-15, pageWidth - (2*margin), 25, 'F');
            pdf.setTextColor(255, 255, 255);
            pdf.text('2. NATURALEZA DE LA LESIÓN', margin + 10, yPos);
            yPos += 20;
            pdf.setTextColor(0, 0, 0);
            
            const naturaleza = [];
            for (let i = 31; i <= 60; i++) {
                const chk = document.getElementById(`i${i}`);
                if (chk && chk.checked) {
                    const label = chk.nextElementSibling;
                    naturaleza.push(label ? label.textContent.trim() : `Opción ${i}`);
                }
            }
            
            if (naturaleza.length > 0) {
                const texto = naturaleza.join(', ');
                const lineas = pdf.splitTextToSize(texto, pageWidth - (2*margin) - 30);
                if (yPos + (lineas.length * 14) > pageHeight - 60) {
                    pdf.addPage();
                    pageNumber++;
                    yPos = 50;
                }
                pdf.text(lineas, margin + 10, yPos);
                yPos += (lineas.length * 14) + 15;
            } else {
                pdf.text('Ninguna naturaleza seleccionada', margin + 10, yPos);
                yPos += 25;
            }

            // Contacto y mecanismo
            checkSpace(80);
            pdf.setFillColor(44, 62, 80);
            pdf.rect(margin, yPos-15, pageWidth - (2*margin), 25, 'F');
            pdf.setTextColor(255, 255, 255);
            pdf.text('3. CONTACTO Y MECANISMO', margin + 10, yPos);
            yPos += 20;
            pdf.setTextColor(0, 0, 0);
            pdf.setFontSize(10);
            
            pdf.setFont('helvetica', 'bold');
            pdf.text('Agencia:', margin + 10, yPos);
            pdf.setFont('helvetica', 'normal');
            pdf.text(document.getElementById('agencia').value || 'No seleccionada', margin + 80, yPos);
            yPos += 15;
            pdf.setFont('helvetica', 'bold');
            pdf.text('Mecanismo:', margin + 10, yPos);
            pdf.setFont('helvetica', 'normal');
            pdf.text(document.getElementById('mecanismo').value || 'No seleccionado', margin + 90, yPos);
            yPos += 25;

            // Causas inmediatas
            checkSpace(80);
            pdf.setFillColor(44, 62, 80);
            pdf.rect(margin, yPos-15, pageWidth - (2*margin), 25, 'F');
            pdf.setTextColor(255, 255, 255);
            pdf.text('4. CAUSAS INMEDIATAS', margin + 10, yPos);
            yPos += 20;
            pdf.setTextColor(0, 0, 0);
            
            pdf.setFont('helvetica', 'bold');
            pdf.text('Práctica Sub-estándar:', margin + 10, yPos);
            pdf.setFont('helvetica', 'normal');
            pdf.text(document.getElementById('practica').value || 'No seleccionada', margin + 150, yPos);
            yPos += 15;
            pdf.setFont('helvetica', 'bold');
            pdf.text('Condición Sub-estándar:', margin + 10, yPos);
            pdf.setFont('helvetica', 'normal');
            pdf.text(document.getElementById('condicion').value || 'No seleccionada', margin + 160, yPos);
            yPos += 25;

            // Factor Personal
            checkSpace(120);
            pdf.setFillColor(44, 62, 80);
            pdf.rect(margin, yPos-15, pageWidth - (2*margin), 25, 'F');
            pdf.setTextColor(255, 255, 255);
            pdf.text('5. FACTOR PERSONAL', margin + 10, yPos);
            yPos += 20;
            pdf.setTextColor(0, 0, 0);
            
            const fp1 = document.getElementById('opcionfp1');
            const subfp1 = document.getElementById('subgrupofp1');
            if (fp1.value) {
                pdf.setFont('helvetica', 'bold');
                pdf.text('Opción 1:', margin + 10, yPos);
                pdf.setFont('helvetica', 'normal');
                const textoFp1 = fp1.options[fp1.selectedIndex]?.text || '';
                const lineasFp1 = pdf.splitTextToSize(textoFp1, 300);
                pdf.text(lineasFp1, margin + 80, yPos);
                yPos += (lineasFp1.length * 14);
                if (subfp1.value) {
                    pdf.setFont('helvetica', 'bold');
                    pdf.text('Subgrupo 1:', margin + 10, yPos);
                    pdf.setFont('helvetica', 'normal');
                    const lineasSub1 = pdf.splitTextToSize(subfp1.value, 300);
                    pdf.text(lineasSub1, margin + 90, yPos);
                    yPos += (lineasSub1.length * 14);
                }
            }
            
            const fp2 = document.getElementById('opcionfp2');
            const subfp2 = document.getElementById('subgrupofp2');
            if (fp2.value) {
                pdf.setFont('helvetica', 'bold');
                pdf.text('Opción 2:', margin + 10, yPos);
                pdf.setFont('helvetica', 'normal');
                const textoFp2 = fp2.options[fp2.selectedIndex]?.text || '';
                const lineasFp2 = pdf.splitTextToSize(textoFp2, 300);
                pdf.text(lineasFp2, margin + 80, yPos);
                yPos += (lineasFp2.length * 14);
                if (subfp2.value) {
                    pdf.setFont('helvetica', 'bold');
                    pdf.text('Subgrupo 2:', margin + 10, yPos);
                    pdf.setFont('helvetica', 'normal');
                    const lineasSub2 = pdf.splitTextToSize(subfp2.value, 300);
                    pdf.text(lineasSub2, margin + 90, yPos);
                    yPos += (lineasSub2.length * 14);
                }
            }
            if (!fp1.value && !fp2.value) {
                pdf.text('Ningún factor personal seleccionado', margin + 10, yPos);
                yPos += 15;
            }
            yPos += 10;

            // Factor de Trabajo
            checkSpace(120);
            pdf.setFillColor(44, 62, 80);
            pdf.rect(margin, yPos-15, pageWidth - (2*margin), 25, 'F');
            pdf.setTextColor(255, 255, 255);
            pdf.text('6. FACTOR DE TRABAJO', margin + 10, yPos);
            yPos += 20;
            pdf.setTextColor(0, 0, 0);
            
            const ft1 = document.getElementById('opcion1');
            const subft1 = document.getElementById('subgrupo1');
            if (ft1.value) {
                pdf.setFont('helvetica', 'bold');
                pdf.text('Opción 1:', margin + 10, yPos);
                pdf.setFont('helvetica', 'normal');
                const textoFt1 = ft1.options[ft1.selectedIndex]?.text || '';
                const lineasFt1 = pdf.splitTextToSize(textoFt1, 300);
                pdf.text(lineasFt1, margin + 80, yPos);
                yPos += (lineasFt1.length * 14);
                if (subft1.value) {
                    pdf.setFont('helvetica', 'bold');
                    pdf.text('Subgrupo 1:', margin + 10, yPos);
                    pdf.setFont('helvetica', 'normal');
                    const lineasSub1 = pdf.splitTextToSize(subft1.value, 300);
                    pdf.text(lineasSub1, margin + 90, yPos);
                    yPos += (lineasSub1.length * 14);
                }
            }
            
            const ft2 = document.getElementById('opcion2');
            const subft2 = document.getElementById('subgrupo2');
            if (ft2.value) {
                pdf.setFont('helvetica', 'bold');
                pdf.text('Opción 2:', margin + 10, yPos);
                pdf.setFont('helvetica', 'normal');
                const textoFt2 = ft2.options[ft2.selectedIndex]?.text || '';
                const lineasFt2 = pdf.splitTextToSize(textoFt2, 300);
                pdf.text(lineasFt2, margin + 80, yPos);
                yPos += (lineasFt2.length * 14);
                if (subft2.value) {
                    pdf.setFont('helvetica', 'bold');
                    pdf.text('Subgrupo 2:', margin + 10, yPos);
                    pdf.setFont('helvetica', 'normal');
                    const lineasSub2 = pdf.splitTextToSize(subft2.value, 300);
                    pdf.text(lineasSub2, margin + 90, yPos);
                    yPos += (lineasSub2.length * 14);
                }
            }
            if (!ft1.value && !ft2.value) {
                pdf.text('Ningún factor de trabajo seleccionado', margin + 10, yPos);
                yPos += 15;
            }
            yPos += 10;

            // Control de Gerencia
            checkSpace(120);
            pdf.setFillColor(44, 62, 80);
            pdf.rect(margin, yPos-15, pageWidth - (2*margin), 25, 'F');
            pdf.setTextColor(255, 255, 255);
            pdf.text('7. CONTROL DE GERENCIA', margin + 10, yPos);
            yPos += 20;
            pdf.setTextColor(0, 0, 0);
            
            const cg1 = document.getElementById('opcioncg1');
            const subcg1 = document.getElementById('subgrupocg1');
            if (cg1.value) {
                pdf.setFont('helvetica', 'bold');
                pdf.text('Opción 1:', margin + 10, yPos);
                pdf.setFont('helvetica', 'normal');
                const textoCg1 = cg1.options[cg1.selectedIndex]?.text || '';
                const lineasCg1 = pdf.splitTextToSize(textoCg1, 300);
                pdf.text(lineasCg1, margin + 80, yPos);
                yPos += (lineasCg1.length * 14);
                if (subcg1.value) {
                    pdf.setFont('helvetica', 'bold');
                    pdf.text('Subgrupo 1:', margin + 10, yPos);
                    pdf.setFont('helvetica', 'normal');
                    const lineasSub1 = pdf.splitTextToSize(subcg1.value, 300);
                    pdf.text(lineasSub1, margin + 90, yPos);
                    yPos += (lineasSub1.length * 14);
                }
            }
            
            const cg2 = document.getElementById('opcioncg2');
            const subcg2 = document.getElementById('subgrupocg2');
            if (cg2.value) {
                pdf.setFont('helvetica', 'bold');
                pdf.text('Opción 2:', margin + 10, yPos);
                pdf.setFont('helvetica', 'normal');
                const textoCg2 = cg2.options[cg2.selectedIndex]?.text || '';
                const lineasCg2 = pdf.splitTextToSize(textoCg2, 300);
                pdf.text(lineasCg2, margin + 80, yPos);
                yPos += (lineasCg2.length * 14);
                if (subcg2.value) {
                    pdf.setFont('helvetica', 'bold');
                    pdf.text('Subgrupo 2:', margin + 10, yPos);
                    pdf.setFont('helvetica', 'normal');
                    const lineasSub2 = pdf.splitTextToSize(subcg2.value, 300);
                    pdf.text(lineasSub2, margin + 90, yPos);
                    yPos += (lineasSub2.length * 14);
                }
            }
            if (!cg1.value && !cg2.value) {
                pdf.text('Ningún control seleccionado', margin + 10, yPos);
                yPos += 15;
            }
            yPos += 15;

            // Firmas
            if (signaturePad1 && !signaturePad1.isEmpty()) {
                if (yPos + 60 > pageHeight - 50) {
                    pdf.addPage();
                    pageNumber++;
                    yPos = 50;
                }
                const canvas1 = document.getElementById('signature1');
                const imgData1 = canvas1.toDataURL('image/png');
                pdf.setFont('helvetica', 'bold');
                pdf.setFontSize(11);
                pdf.text('Firma del Investigador:', margin, yPos);
                yPos += 10;
                pdf.addImage(imgData1, 'PNG', margin, yPos, 180, 50);
                yPos += 60;
            }
            
            if (signaturePad2 && !signaturePad2.isEmpty()) {
                if (yPos + 60 > pageHeight - 50) {
                    pdf.addPage();
                    pageNumber++;
                    yPos = 50;
                }
                const canvas2 = document.getElementById('signature2');
                const imgData2 = canvas2.toDataURL('image/png');
                pdf.setFont('helvetica', 'bold');
                pdf.text('Firma del Supervisor:', margin, yPos);
                yPos += 10;
                pdf.addImage(imgData2, 'PNG', margin, yPos, 180, 50);
                yPos += 60;
            }

            // Pie de página
            if (yPos + 40 < pageHeight - 30) {
                yPos = pageHeight - 60;
            } else {
                pdf.addPage();
                yPos = pageHeight - 60;
            }
            
            pdf.setDrawColor(200, 200, 200);
            pdf.line(margin, yPos, pageWidth - margin, yPos);
            pdf.setFontSize(8);
            pdf.setTextColor(100, 100, 100);
            pdf.text('Documento generado por SCAT System - Análisis de Causa Raíz', pageWidth/2, yPos + 10, { align: 'center' });
            pdf.text(`Elaborado por: Jeferson_QT | jeferson7316@hotmail.com`, pageWidth/2, yPos + 18, { align: 'center' });
            pdf.text(`Página ${pageNumber}`, pageWidth - 60, yPos + 18);

            pdf.save(`SCAT_${new Date().toISOString().slice(0,10)}.pdf`);
        }

        // ============================================
        // EVENT LISTENERS
        // ============================================
        document.addEventListener('DOMContentLoaded', function() {
            initSignatures();
            
            document.getElementById("opcionfp1").addEventListener("change", function() {
                cargarSubgrupofp(this, "subgrupofp1");
            });
            document.getElementById("opcionfp2").addEventListener("change", function() {
                cargarSubgrupofp(this, "subgrupofp2");
            });
            
            document.getElementById("opcion1").addEventListener("change", function() {
                cargarSubgrupo(this, "subgrupo1");
            });
            document.getElementById("opcion2").addEventListener("change", function() {
                cargarSubgrupo(this, "subgrupo2");
            });
            
            document.getElementById("opcioncg1").addEventListener("change", function() {
                cargarSubgrupocg(this, "subgrupocg1");
            });
            document.getElementById("opcioncg2").addEventListener("change", function() {
                cargarSubgrupocg(this, "subgrupocg2");
            });
        });
    </script>
</body>
</html>
