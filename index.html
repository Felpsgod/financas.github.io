<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Meu Controle Financeiro</title>
    <!-- Firebase SDK -->
    <script src="https://www.gstatic.com/firebasejs/9.22.0/firebase-app-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/9.22.0/firebase-database-compat.js"></script>
    <!-- Bootstrap 5 -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        :root {
            --color-primary: #348888;
            --color-secondary: #22BABB;
            --color-accent: #9EF8EE;
            --color-warning: #FA7F08;
            --color-danger: #F24405;
            --text-light: #ffffff;
            --text-dark: #333333;
            --card-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #e4edf5 100%);
            font-family: 'Segoe UI', 'Roboto', sans-serif;
            color: var(--text-dark);
            padding-bottom: 80px;
            min-height: 100vh;
        }
        
        .header {
            background: linear-gradient(135deg, var(--color-primary), var(--color-secondary));
            color: var(--text-light);
            padding: 20px 0;
            margin-bottom: 20px;
            box-shadow: 0 4px 12px rgba(52, 136, 136, 0.3);
        }
        
        .header h1 {
            font-size: 1.8rem;
            margin-bottom: 5px;
            font-weight: 700;
        }
        
        .header p {
            font-size: 0.9rem;
            opacity: 0.9;
            margin-bottom: 0;
        }
        
        .card-finance {
            border-radius: 15px;
            border: none;
            box-shadow: var(--card-shadow);
            margin-bottom: 15px;
            transition: all 0.3s ease;
            height: 100%;
            min-height: 280px;
        }
        
        .card-finance:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }
        
        .card-header-custom {
            background: linear-gradient(135deg, var(--color-primary), var(--color-secondary));
            color: white;
            border-radius: 15px 15px 0 0 !important;
            padding: 12px 15px;
            font-weight: 600;
            font-size: 1rem;
        }
        
        .card-body {
            padding: 15px;
        }
        
        .progress {
            height: 8px;
            margin: 12px 0;
            border-radius: 4px;
        }
        
        .progress-bar {
            border-radius: 4px;
        }
        
        .btn-custom-primary {
            background-color: var(--color-primary);
            color: white;
            border: none;
            padding: 8px 16px;
            border-radius: 8px;
            font-weight: 500;
            font-size: 0.9rem;
            transition: all 0.3s;
        }
        
        .btn-custom-primary:hover {
            background-color: var(--color-secondary);
            transform: scale(1.03);
        }
        
        .btn-custom-warning {
            background-color: var(--color-warning);
            color: white;
            border: none;
            padding: 8px 16px;
            border-radius: 8px;
            font-weight: 500;
            font-size: 0.9rem;
            transition: all 0.3s;
        }
        
        .btn-custom-danger {
            background-color: var(--color-danger);
            color: white;
            border: none;
            padding: 8px 16px;
            border-radius: 8px;
            font-weight: 500;
            font-size: 0.9rem;
            transition: all 0.3s;
        }
        
        .btn-custom-success {
            background-color: var(--color-primary);
            color: white;
            border: none;
            padding: 8px 16px;
            border-radius: 8px;
            font-weight: 500;
            font-size: 0.9rem;
            transition: all 0.3s;
        }
        
        .btn-small {
            padding: 4px 10px !important;
            font-size: 0.8rem !important;
            margin: 2px;
        }
        
        .value-display {
            font-size: 1.4rem;
            font-weight: 700;
            color: var(--color-primary);
            text-align: center;
            margin: 5px 0;
        }
        
        .counter-display {
            font-size: 1.8rem;
            font-weight: 800;
            color: var(--color-secondary);
            text-align: center;
            margin: 10px 0;
        }
        
        .loading-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(255, 255, 255, 0.95);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 9999;
            flex-direction: column;
        }
        
        .footer {
            position: fixed;
            bottom: 0;
            width: 100%;
            background: white;
            padding: 12px 15px;
            box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.1);
            border-top: 3px solid var(--color-primary);
            z-index: 100;
        }
        
        .expense-item {
            border-left: 4px solid var(--color-warning);
            padding-left: 10px;
            margin-bottom: 10px;
            padding: 8px;
            background: #f8f9fa;
            border-radius: 5px;
        }
        
        .loan-item {
            border-left: 4px solid var(--color-secondary);
            padding-left: 10px;
            margin-bottom: 10px;
            padding: 8px;
            background: #f8f9fa;
            border-radius: 5px;
        }
        
        .modal-header-custom {
            background: linear-gradient(135deg, var(--color-primary), var(--color-secondary));
            color: white;
            border-radius: 15px 15px 0 0;
        }
        
        /* Responsividade para iPhone */
        @media (max-width: 768px) {
            .header h1 {
                font-size: 1.5rem;
            }
            
            .header p {
                font-size: 0.8rem;
            }
            
            .card-body {
                padding: 12px;
            }
            
            .value-display {
                font-size: 1.2rem;
            }
            
            .counter-display {
                font-size: 1.5rem;
            }
            
            .btn-custom-primary, .btn-custom-warning, .btn-custom-danger, .btn-custom-success {
                padding: 6px 12px;
                font-size: 0.85rem;
            }
            
            .row-cols-md-2 > * {
                flex: 0 0 auto;
                width: 100%;
            }
        }
        
        @media (max-width: 576px) {
            .container {
                padding-left: 10px;
                padding-right: 10px;
            }
            
            .header {
                padding: 15px 0;
            }
            
            .card-finance {
                margin-bottom: 12px;
            }
        }
        
        /* Grid para cards lado a lado */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 15px;
        }
        
        /* Toast notifications */
        .toast-custom {
            position: fixed;
            top: 20px;
            right: 20px;
            z-index: 1000;
            min-width: 250px;
        }
        
        .total-monthly {
            background: linear-gradient(135deg, var(--color-primary), var(--color-secondary));
            color: white;
            padding: 10px 15px;
            border-radius: 10px;
            font-weight: 600;
            margin-top: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <!-- Loading Overlay -->
    <div id="loadingOverlay" class="loading-overlay">
        <div class="spinner-border" style="color: var(--color-primary);" role="status">
            <span class="visually-hidden">Carregando...</span>
        </div>
        <p class="mt-3" style="color: var(--color-primary); font-weight: 500;">Conectando ao seu controle financeiro...</p>
    </div>

    <!-- Toast Notifications -->
    <div id="toastContainer" class="toast-custom"></div>

    <!-- Header -->
    <div class="header">
        <div class="container">
            <div class="d-flex justify-content-between align-items-center">
                <div>
                    <h1>💰 Controle Financeiro Pessoal</h1>
                    <p>Controle seus financiamentos, empréstimos e despesas</p>
                </div>
                <div id="lastUpdate" class="text-end" style="font-size: 0.8rem; opacity: 0.8;">
                    Última atualização: <span id="updateTime">--:--</span>
                </div>
            </div>
        </div>
    </div>

    <div class="container">
        <!-- Cards em Grid -->
        <div class="card-grid">
            <!-- Card 1: Financiamento do Apartamento -->
            <div class="card card-finance">
                <div class="card-header card-header-custom d-flex justify-content-between align-items-center">
                    <span>🏠 Financiamento Apartamento</span>
                    <button class="btn btn-sm btn-light" onclick="showEditApartmentModal()" title="Editar Financiamento">
                        <small>Editar</small>
                    </button>
                </div>
                <div class="card-body">
                    <div class="counter-display">
                        <span id="apartmentPaidCount">0</span>/<span id="apartmentTotalCount">360</span>
                    </div>
                    <div class="text-center mb-2">
                        <small>Parcelas pagas / total</small>
                    </div>
                    
                    <div class="value-display">R$ <span id="apartmentMonthly">1.840,00</span></div>
                    <div class="text-center mb-3">
                        <small>Valor da parcela</small>
                    </div>
                    
                    <div class="progress">
                        <div id="apartmentProgress" class="progress-bar" role="progressbar" style="width: 0%; background-color: var(--color-primary);"></div>
                    </div>
                    <div class="text-center mb-3">
                        <small><span id="apartmentPercentage">0</span>% concluído</small>
                    </div>
                    
                    <div class="d-grid gap-2">
                        <button class="btn btn-custom-success" onclick="payApartmentInstallment()">
                            ✅ Pagar Parcela
                        </button>
                        <button class="btn btn-custom-warning" onclick="returnApartmentInstallment()">
                            ↩️ Retornar Parcela
                        </button>
                    </div>
                    
                    <div class="total-monthly mt-3">
                        Total Mês: R$ <span id="apartmentTotalMonth">1.840,00</span>
                    </div>
                </div>
            </div>

            <!-- Card 2: Entrada do Apartamento -->
            <div class="card card-finance">
                <div class="card-header card-header-custom">
                    <span>🏠 Entrada do Apartamento</span>
                </div>
                <div class="card-body">
                    <div class="counter-display">
                        <span id="entryPaidCount">0</span>/<span id="entryTotalCount">28</span>
                    </div>
                    <div class="text-center mb-2">
                        <small>Parcelas pagas / total</small>
                    </div>
                    
                    <div class="value-display">R$ <span id="entryMonthly">300,00</span></div>
                    <div class="text-center mb-3">
                        <small>Valor da parcela</small>
                    </div>
                    
                    <div class="progress">
                        <div id="entryProgress" class="progress-bar" role="progressbar" style="width: 0%; background-color: var(--color-secondary);"></div>
                    </div>
                    <div class="text-center mb-3">
                        <small><span id="entryPercentage">0</span>% concluído</small>
                    </div>
                    
                    <div class="d-grid gap-2">
                        <button class="btn btn-custom-success" onclick="payEntryInstallment()">
                            ✅ Pagar Parcela
                        </button>
                        <button class="btn btn-custom-warning" onclick="returnEntryInstallment()">
                            ↩️ Retornar Parcela
                        </button>
                    </div>
                    
                    <div class="total-monthly mt-3">
                        Total Pago: R$ <span id="entryTotalPaid">0,00</span>
                    </div>
                </div>
            </div>

            <!-- Card 3: Financiamento do Carro -->
            <div class="card card-finance">
                <div class="card-header card-header-custom d-flex justify-content-between align-items-center">
                    <span>🚗 Financiamento Carro</span>
                    <button class="btn btn-sm btn-light" onclick="showEditCarModal()" title="Editar Financiamento">
                        <small>Editar</small>
                    </button>
                </div>
                <div class="card-body">
                    <div class="counter-display">
                        <span id="carPaidCount">0</span>/<span id="carTotalCount">60</span>
                    </div>
                    <div class="text-center mb-2">
                        <small>Parcelas pagas / total</small>
                    </div>
                    
                    <div class="value-display">R$ <span id="carMonthly">1.250,00</span></div>
                    <div class="text-center mb-3">
                        <small>Valor da parcela</small>
                    </div>
                    
                    <div class="progress">
                        <div id="carProgress" class="progress-bar" role="progressbar" style="width: 0%; background-color: var(--color-warning);"></div>
                    </div>
                    <div class="text-center mb-3">
                        <small><span id="carPercentage">0</span>% concluído</small>
                    </div>
                    
                    <div class="d-grid gap-2">
                        <button class="btn btn-custom-success" onclick="payCarInstallment()">
                            ✅ Pagar Parcela
                        </button>
                        <button class="btn btn-custom-warning" onclick="returnCarInstallment()">
                            ↩️ Retornar Parcela
                        </button>
                    </div>
                    
                    <div class="total-monthly mt-3">
                        Total Mês: R$ <span id="carTotalMonth">1.250,00</span>
                    </div>
                </div>
            </div>

            <!-- Card 4: Despesas do Apartamento -->
            <div class="card card-finance">
                <div class="card-header card-header-custom d-flex justify-content-between align-items-center">
                    <span>🏠 Despesas do Apartamento</span>
                    <button class="btn btn-sm btn-light" onclick="showEditExpensesModal()" title="Editar Despesas">
                        <small>Editar</small>
                    </button>
                </div>
                <div class="card-body">
                    <div class="mb-3">
                        <div class="d-flex justify-content-between mb-2">
                            <span>Condomínio:</span>
                            <span>R$ <span id="condominioValue">450,00</span></span>
                        </div>
                        <div class="d-flex justify-content-between mb-2">
                            <span>Água:</span>
                            <span>R$ <span id="aguaValue">120,00</span></span>
                        </div>
                        <div class="d-flex justify-content-between mb-3">
                            <span>Energia:</span>
                            <span>R$ <span id="energiaValue">250,00</span></span>
                        </div>
                    </div>
                    
                    <div class="value-display">R$ <span id="totalExpenses">820,00</span></div>
                    <div class="text-center mb-3">
                        <small>Total das despesas</small>
                    </div>
                    
                    <div class="mt-4">
                        <div class="d-flex justify-content-between mb-2">
                            <span>Total com Financiamento:</span>
                            <span>R$ <span id="apartmentFinancing">1.840,00</span></span>
                        </div>
                        <div class="d-flex justify-content-between mb-2">
                            <span>Total com Despesas:</span>
                            <span>R$ <span id="apartmentExpensesTotal">820,00</span></span>
                        </div>
                        <div class="total-monthly mt-3">
                            <strong>TOTAL APARTAMENTO:</strong> R$ <span id="apartmentGrandTotal">2.660,00</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Card 5: Empréstimos -->
            <div class="card card-finance">
                <div class="card-header card-header-custom d-flex justify-content-between align-items-center">
                    <span>📄 Empréstimos</span>
                    <button class="btn btn-sm btn-light" onclick="showAddLoanModal()" title="Adicionar Empréstimo">
                        <small>+ Novo</small>
                    </button>
                </div>
                <div class="card-body" style="overflow-y: auto; max-height: 250px;">
                    <div id="loansContainer">
                        <p class="text-muted text-center" style="font-size: 0.9rem;">Nenhum empréstimo cadastrado</p>
                    </div>
                </div>
            </div>

            <!-- Card 6: Cartão de Crédito -->
            <div class="card card-finance">
                <div class="card-header card-header-custom d-flex justify-content-between align-items-center">
                    <span>💳 Cartão de Crédito</span>
                    <button class="btn btn-sm btn-light" onclick="showAddCreditExpenseModal()" title="Adicionar Despesa">
                        <small>+ Nova</small>
                    </button>
                </div>
                <div class="card-body" style="overflow-y: auto; max-height: 250px;">
                    <div id="creditCardContainer">
                        <p class="text-muted text-center" style="font-size: 0.9rem;">Nenhuma despesa no cartão</p>
                    </div>
                    <div class="total-monthly mt-2">
                        Total: R$ <span id="creditCardTotal">0,00</span>
                    </div>
                </div>
            </div>

            <!-- Card 7: Despesas Gerais -->
            <div class="card card-finance">
                <div class="card-header card-header-custom d-flex justify-content-between align-items-center">
                    <span>📋 Despesas Gerais</span>
                    <button class="btn btn-sm btn-light" onclick="showAddExpenseModal()" title="Adicionar Despesa">
                        <small>+ Nova</small>
                    </button>
                </div>
                <div class="card-body" style="overflow-y: auto; max-height: 250px;">
                    <div id="expensesContainer">
                        <p class="text-muted text-center" style="font-size: 0.9rem;">Nenhuma despesa geral</p>
                    </div>
                    <div class="total-monthly mt-2">
                        Total: R$ <span id="expensesTotal">0,00</span>
                    </div>
                </div>
            </div>

            <!-- Card 8: Resumo Financeiro Mensal -->
            <div class="card card-finance">
                <div class="card-header card-header-custom">
                    <span>📊 Resumo do Mês</span>
                </div>
                <div class="card-body">
                    <div class="mb-3">
                        <div class="d-flex justify-content-between mb-2">
                            <span>Apartamento:</span>
                            <span>R$ <span id="resumoApartment">2.660,00</span></span>
                        </div>
                        <div class="d-flex justify-content-between mb-2">
                            <span>Carro:</span>
                            <span>R$ <span id="resumoCar">1.250,00</span></span>
                        </div>
                        <div class="d-flex justify-content-between mb-2">
                            <span>Empréstimos:</span>
                            <span>R$ <span id="resumoLoans">0,00</span></span>
                        </div>
                        <div class="d-flex justify-content-between mb-2">
                            <span>Cartão de Crédito:</span>
                            <span>R$ <span id="resumoCredit">0,00</span></span>
                        </div>
                        <div class="d-flex justify-content-between mb-3">
                            <span>Outras Despesas:</span>
                            <span>R$ <span id="resumoExpenses">0,00</span></span>
                        </div>
                    </div>
                    
                    <div class="value-display" style="color: var(--color-danger);">R$ <span id="resumoTotal">3.910,00</span></div>
                    <div class="text-center mb-3">
                        <small>Total mensal estimado</small>
                    </div>
                    
                    <div class="mt-3">
                        <div class="d-flex justify-content-between mb-2">
                            <small>Parcelas restantes (Apto):</small>
                            <small><span id="resumoAptoRestantes">360</span></small>
                        </div>
                        <div class="d-flex justify-content-between mb-2">
                            <small>Parcelas restantes (Carro):</small>
                            <small><span id="resumoCarroRestantes">60</span></small>
                        </div>
                        <div class="d-flex justify-content-between">
                            <small>Economia mensal:</small>
                            <small>R$ <span id="resumoEconomia">0,00</span></small>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <div class="footer">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-8">
                    <small style="color: var(--color-primary); font-weight: 500;">
                        <span id="dataStatus">🟢 Dados sincronizados em tempo real</span>
                    </small>
                </div>
                <div class="col-4 text-end">
                    <button class="btn btn-sm btn-custom-primary" onclick="exportData()" title="Exportar dados">
                        📥 Exportar
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modais -->
    <!-- Modal Editar Financiamento Apartamento -->
    <div class="modal fade" id="editApartmentModal" tabindex="-1">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header modal-header-custom">
                    <h5 class="modal-title">Editar Financiamento do Apartamento</h5>
                    <button type="button" class="btn-close btn-close-white" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body">
                    <div class="mb-3">
                        <label class="form-label">Parcelas Pagas:</label>
                        <input type="number" id="editApartmentPaid" class="form-control" min="0" max="360">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Valor da Parcela: R$</label>
                        <input type="number" id="editApartmentValue" class="form-control" step="0.01">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Total de Parcelas:</label>
                        <input type="number" id="editApartmentTotal" class="form-control" min="1" value="360">
                    </div>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancelar</button>
                    <button type="button" class="btn btn-custom-primary" onclick="saveApartmentEdit()">Salvar Alterações</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Editar Despesas do Apartamento -->
    <div class="modal fade" id="editExpensesModal" tabindex="-1">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header modal-header-custom">
                    <h5 class="modal-title">Editar Despesas do Apartamento</h5>
                    <button type="button" class="btn-close btn-close-white" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body">
                    <div class="mb-3">
                        <label class="form-label">Condomínio: R$</label>
                        <input type="number" id="editCondominio" class="form-control" step="0.01">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Água: R$</label>
                        <input type="number" id="editAgua" class="form-control" step="0.01">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Energia: R$</label>
                        <input type="number" id="editEnergia" class="form-control" step="0.01">
                    </div>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancelar</button>
                    <button type="button" class="btn btn-custom-primary" onclick="saveExpensesEdit()">Salvar Despesas</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Adicionar Empréstimo -->
    <div class="modal fade" id="addLoanModal" tabindex="-1">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header modal-header-custom">
                    <h5 class="modal-title">Adicionar Empréstimo</h5>
                    <button type="button" class="btn-close btn-close-white" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body">
                    <div class="mb-3">
                        <label class="form-label">Nome do Empréstimo:</label>
                        <input type="text" id="loanName" class="form-control" placeholder="Ex: Empréstimo Pessoal">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Valor Total: R$</label>
                        <input type="number" id="loanTotal" class="form-control" step="0.01" value="10000.00">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Valor da Parcela: R$</label>
                        <input type="number" id="loanMonthly" class="form-control" step="0.01" value="500.00">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Total de Parcelas:</label>
                        <input type="number" id="loanInstallments" class="form-control" value="24">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Parcelas Já Pagas:</label>
                        <input type="number" id="loanPaid" class="form-control" value="0">
                    </div>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancelar</button>
                    <button type="button" class="btn btn-custom-primary" onclick="addNewLoan()">Adicionar Empréstimo</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Editar Empréstimo -->
    <div class="modal fade" id="editLoanModal" tabindex="-1">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header modal-header-custom">
                    <h5 class="modal-title">Editar Empréstimo</h5>
                    <button type="button" class="btn-close btn-close-white" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body" id="editLoanModalBody">
                    <!-- Conteúdo preenchido dinamicamente -->
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Adicionar Despesa Cartão de Crédito -->
    <div class="modal fade" id="addCreditExpenseModal" tabindex="-1">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header modal-header-custom">
                    <h5 class="modal-title">Adicionar Despesa no Cartão</h5>
                    <button type="button" class="btn-close btn-close-white" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body">
                    <div class="mb-3">
                        <label class="form-label">Descrição:</label>
                        <input type="text" id="creditExpenseName" class="form-control" placeholder="Ex: Supermercado">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Valor: R$</label>
                        <input type="number" id="creditExpenseAmount" class="form-control" step="0.01" value="0.00">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Data:</label>
                        <input type="date" id="creditExpenseDate" class="form-control">
                    </div>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancelar</button>
                    <button type="button" class="btn btn-custom-primary" onclick="addNewCreditExpense()">Adicionar Despesa</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Modal Adicionar Despesa Geral -->
    <div class="modal fade" id="addExpenseModal" tabindex="-1">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header modal-header-custom">
                    <h5 class="modal-title">Adicionar Despesa Geral</h5>
                    <button type="button" class="btn-close btn-close-white" data-bs-dismiss="modal"></button>
                </div>
                <div class="modal-body">
                    <div class="mb-3">
                        <label class="form-label">Descrição:</label>
                        <input type="text" id="expenseName" class="form-control" placeholder="Ex: Academia, Transporte">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Valor: R$</label>
                        <input type="number" id="expenseAmount" class="form-control" step="0.01" value="0.00">
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Categoria:</label>
                        <select id="expenseCategory" class="form-control">
                            <option value="alimentacao">Alimentação</option>
                            <option value="transporte">Transporte</option>
                            <option value="lazer">Lazer</option>
                            <option value="saude">Saúde</option>
                            <option value="outros">Outros</option>
                        </select>
                    </div>
                    <div class="mb-3">
                        <label class="form-label">Data:</label>
                        <input type="date" id="expenseDate" class="form-control">
                    </div>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancelar</button>
                    <button type="button" class="btn btn-custom-primary" onclick="addNewExpense()">Adicionar Despesa</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    
    <script>
        // Configuração do Firebase (USE SUAS PRÓPRIAS CREDENCIAIS)
        const firebaseConfig = {
            apiKey: "AIzaSyCz3Q8qH2oHkK7v9QkL-6mX6JZ4Xq8Y9v0",
            authDomain: "financas-8d957.firebaseapp.com",
            databaseURL: "https://financas-8d957-default-rtdb.firebaseio.com",
            projectId: "financas-8d957",
            storageBucket: "financas-8d957.appspot.com",
            messagingSenderId: "123456789012",
            appId: "1:123456789012:web:abcdef1234567890"
        };

        // Inicializar Firebase
        firebase.initializeApp(firebaseConfig);
        const database = firebase.database();
        
        // Estado global da aplicação
        let financialData = {
            apartment: {
                totalInstallments: 360,
                installmentValue: 1840,
                paidInstallments: 0
            },
            entry: {
                totalInstallments: 28,
                installmentValue: 300,
                paidInstallments: 0
            },
            car: {
                totalInstallments: 60,
                installmentValue: 1250,
                paidInstallments: 0
            },
            expenses: {
                condominium: 450,
                water: 120,
                energy: 250
            },
            loans: [],
            creditCard: [],
            generalExpenses: []
        };

        // Inicializar a aplicação
        document.addEventListener('DOMContentLoaded', function() {
            // Configurar data atual nos modais
            const today = new Date().toISOString().split('T')[0];
            document.getElementById('creditExpenseDate').value = today;
            document.getElementById('expenseDate').value = today;
            
            // Carregar dados do Firebase em tempo real
            setupRealtimeListeners();
            
            // Atualizar interface inicial
            updateAllDisplays();
            updateResumo();
            
            // Esconder loading após carregar
            setTimeout(() => {
                document.getElementById('loadingOverlay').style.display = 'none';
            }, 1000);
            
            // Atualizar hora
            updateTime();
            setInterval(updateTime, 60000);
        });

        // Configurar listeners em tempo real
        function setupRealtimeListeners() {
            // Apartamento
            database.ref('apartment').on('value', (snapshot) => {
                if (snapshot.exists()) {
                    financialData.apartment = snapshot.val();
                    updateApartmentDisplay();
                    updateResumo();
                    showToast('Dados do apartamento atualizados', 'success');
                }
            });
            
            // Entrada
            database.ref('entry').on('value', (snapshot) => {
                if (snapshot.exists()) {
                    financialData.entry = snapshot.val();
                    updateEntryDisplay();
                    updateResumo();
                }
            });
            
            // Carro
            database.ref('car').on('value', (snapshot) => {
                if (snapshot.exists()) {
                    financialData.car = snapshot.val();
                    updateCarDisplay();
                    updateResumo();
                }
            });
            
            // Despesas
            database.ref('expenses').on('value', (snapshot) => {
                if (snapshot.exists()) {
                    financialData.expenses = snapshot.val();
                    updateExpensesDisplay();
                    updateResumo();
                }
            });
            
            // Empréstimos
            database.ref('loans').on('value', (snapshot) => {
                if (snapshot.exists()) {
                    financialData.loans = snapshot.val();
                    renderLoans();
                    updateResumo();
                }
            });
            
            // Cartão de Crédito
            database.ref('creditCard').on('value', (snapshot) => {
                if (snapshot.exists()) {
                    financialData.creditCard = snapshot.val();
                    renderCreditCard();
                    updateResumo();
                }
            });
            
            // Despesas Gerais
            database.ref('generalExpenses').on('value', (snapshot) => {
                if (snapshot.exists()) {
                    financialData.generalExpenses = snapshot.val();
                    renderGeneralExpenses();
                    updateResumo();
                }
            });
        }

        // Funções para o Financiamento do Apartamento
        function updateApartmentDisplay() {
            const apt = financialData.apartment;
            const percentage = apt.totalInstallments > 0 ? 
                Math.round((apt.paidInstallments / apt.totalInstallments) * 100) : 0;
            
            document.getElementById('apartmentPaidCount').textContent = apt.paidInstallments;
            document.getElementById('apartmentTotalCount').textContent = apt.totalInstallments;
            document.getElementById('apartmentMonthly').textContent = formatCurrency(apt.installmentValue);
            document.getElementById('apartmentProgress').style.width = `${percentage}%`;
            document.getElementById('apartmentPercentage').textContent = percentage;
            document.getElementById('apartmentFinancing').textContent = formatCurrency(apt.installmentValue);
            document.getElementById('apartmentTotalMonth').textContent = formatCurrency(apt.installmentValue);
            
            updateApartmentTotal();
        }

        function payApartmentInstallment() {
            if (financialData.apartment.paidInstallments < financialData.apartment.totalInstallments) {
                financialData.apartment.paidInstallments++;
                saveToFirebase('apartment', financialData.apartment);
                showToast('Parcela do apartamento registrada!', 'success');
            } else {
                showToast('Todas as parcelas já foram pagas!', 'info');
            }
        }

        function returnApartmentInstallment() {
            if (financialData.apartment.paidInstallments > 0) {
                financialData.apartment.paidInstallments--;
                saveToFirebase('apartment', financialData.apartment);
                showToast('Parcela retornada com sucesso!', 'warning');
            } else {
                showToast('Não há parcelas para retornar!', 'info');
            }
        }

        function showEditApartmentModal() {
            document.getElementById('editApartmentPaid').value = financialData.apartment.paidInstallments;
            document.getElementById('editApartmentValue').value = financialData.apartment.installmentValue;
            document.getElementById('editApartmentTotal').value = financialData.apartment.totalInstallments;
            
            new bootstrap.Modal(document.getElementById('editApartmentModal')).show();
        }

        function saveApartmentEdit() {
            financialData.apartment.paidInstallments = parseInt(document.getElementById('editApartmentPaid').value) || 0;
            financialData.apartment.installmentValue = parseFloat(document.getElementById('editApartmentValue').value) || 1840;
            financialData.apartment.totalInstallments = parseInt(document.getElementById('editApartmentTotal').value) || 360;
            
            saveToFirebase('apartment', financialData.apartment);
            bootstrap.Modal.getInstance(document.getElementById('editApartmentModal')).hide();
            showToast('Financiamento atualizado!', 'success');
        }

        // Funções para a Entrada do Apartamento
        function updateEntryDisplay() {
            const entry = financialData.entry;
            const percentage = entry.totalInstallments > 0 ? 
                Math.round((entry.paidInstallments / entry.totalInstallments) * 100) : 0;
            const totalPaid = entry.installmentValue * entry.paidInstallments;
            
            document.getElementById('entryPaidCount').textContent = entry.paidInstallments;
            document.getElementById('entryTotalCount').textContent = entry.totalInstallments;
            document.getElementById('entryMonthly').textContent = formatCurrency(entry.installmentValue);
            document.getElementById('entryProgress').style.width = `${percentage}%`;
            document.getElementById('entryPercentage').textContent = percentage;
            document.getElementById('entryTotalPaid').textContent = formatCurrency(totalPaid);
        }

        function payEntryInstallment() {
            if (financialData.entry.paidInstallments < financialData.entry.totalInstallments) {
                financialData.entry.paidInstallments++;
                saveToFirebase('entry', financialData.entry);
                showToast('Parcela da entrada registrada!', 'success');
            } else {
                showToast('Todas as parcelas da entrada já foram pagas!', 'info');
            }
        }

        function returnEntryInstallment() {
            if (financialData.entry.paidInstallments > 0) {
                financialData.entry.paidInstallments--;
                saveToFirebase('entry', financialData.entry);
                showToast('Parcela da entrada retornada!', 'warning');
            } else {
                showToast('Não há parcelas para retornar!', 'info');
            }
        }

        // Funções para o Financiamento do Carro
        function updateCarDisplay() {
            const car = financialData.car;
            const percentage = car.totalInstallments > 0 ? 
                Math.round((car.paidInstallments / car.totalInstallments) * 100) : 0;
            
            document.getElementById('carPaidCount').textContent = car.paidInstallments;
            document.getElementById('carTotalCount').textContent = car.totalInstallments;
            document.getElementById('carMonthly').textContent = formatCurrency(car.installmentValue);
            document.getElementById('carProgress').style.width = `${percentage}%`;
            document.getElementById('carPercentage').textContent = percentage;
            document.getElementById('carTotalMonth').textContent = formatCurrency(car.installmentValue);
        }

        function payCarInstallment() {
            if (financialData.car.paidInstallments < financialData.car.totalInstallments) {
                financialData.car.paidInstallments++;
                saveToFirebase('car', financialData.car);
                showToast('Parcela do carro registrada!', 'success');
            } else {
                showToast('Todas as parcelas do carro já foram pagas!', 'info');
            }
        }

        function returnCarInstallment() {
            if (financialData.car.paidInstallments > 0) {
                financialData.car.paidInstallments--;
                saveToFirebase('car', financialData.car);
                showToast('Parcela do carro retornada!', 'warning');
            } else {
                showToast('Não há parcelas para retornar!', 'info');
            }
        }

        function showEditCarModal() {
            // Implementar modal similar ao do apartamento
            showToast('Funcionalidade em desenvolvimento', 'info');
        }

        // Funções para Despesas do Apartamento
        function updateExpensesDisplay() {
            const exp = financialData.expenses;
            const total = exp.condominium + exp.water + exp.energy;
            
            document.getElementById('condominioValue').textContent = formatCurrency(exp.condominium);
            document.getElementById('aguaValue').textContent = formatCurrency(exp.water);
            document.getElementById('energiaValue').textContent = formatCurrency(exp.energy);
            document.getElementById('totalExpenses').textContent = formatCurrency(total);
            document.getElementById('apartmentExpensesTotal').textContent = formatCurrency(total);
            
            updateApartmentTotal();
        }

        function updateApartmentTotal() {
            const aptValue = financialData.apartment.installmentValue;
            const expTotal = financialData.expenses.condominium + 
                           financialData.expenses.water + 
                           financialData.expenses.energy;
            const total = aptValue + expTotal;
            
            document.getElementById('apartmentGrandTotal').textContent = formatCurrency(total);
        }

        function showEditExpensesModal() {
            document.getElementById('editCondominio').value = financialData.expenses.condominium;
            document.getElementById('editAgua').value = financialData.expenses.water;
            document.getElementById('editEnergia').value = financialData.expenses.energy;
            
            new bootstrap.Modal(document.getElementById('editExpensesModal')).show();
        }

        function saveExpensesEdit() {
            financialData.expenses.condominium = parseFloat(document.getElementById('editCondominio').value) || 0;
            financialData.expenses.water = parseFloat(document.getElementById('editAgua').value) || 0;
            financialData.expenses.energy = parseFloat(document.getElementById('editEnergia').value) || 0;
            
            saveToFirebase('expenses', financialData.expenses);
            bootstrap.Modal.getInstance(document.getElementById('editExpensesModal')).hide();
            showToast('Despesas atualizadas!', 'success');
        }

        // Funções para Empréstimos
        function showAddLoanModal() {
            new bootstrap.Modal(document.getElementById('addLoanModal')).show();
        }

        function addNewLoan() {
            const name = document.getElementById('loanName').value || 'Empréstimo';
            const total = parseFloat(document.getElementById('loanTotal').value) || 0;
            const monthly = parseFloat(document.getElementById('loanMonthly').value) || 0;
            const installments = parseInt(document.getElementById('loanInstallments').value) || 0;
            const paid = parseInt(document.getElementById('loanPaid').value) || 0;
            
            if (total <= 0 || monthly <= 0) {
                showToast('Preencha valores válidos!', 'danger');
                return;
            }
            
            const newLoan = {
                id: Date.now(),
                name: name,
                totalAmount: total,
                monthlyPayment: monthly,
                totalInstallments: installments,
                paidInstallments: paid
            };
            
            financialData.loans.push(newLoan);
            saveToFirebase('loans', financialData.loans);
            
            bootstrap.Modal.getInstance(document.getElementById('addLoanModal')).hide();
            showToast('Empréstimo adicionado!', 'success');
        }

        function renderLoans() {
            const container = document.getElementById('loansContainer');
            
            if (!financialData.loans || financialData.loans.length === 0) {
                container.innerHTML = '<p class="text-muted text-center" style="font-size: 0.9rem;">Nenhum empréstimo cadastrado</p>';
                return;
            }
            
            let html = '';
            
            financialData.loans.forEach(loan => {
                const percentage = loan.totalInstallments > 0 ? 
                    Math.round((loan.paidInstallments / loan.totalInstallments) * 100) : 0;
                const remaining = loan.totalAmount - (loan.monthlyPayment * loan.paidInstallments);
                
                html += `
                    <div class="loan-item">
                        <div class="d-flex justify-content-between align-items-start">
                            <div style="flex: 1;">
                                <strong style="font-size: 0.9rem;">${loan.name}</strong>
                                <div style="font-size: 0.8rem;">
                                    <div>Parcela: R$ ${formatCurrency(loan.monthlyPayment)}</div>
                                    <div>${loan.paidInstallments}/${loan.totalInstallments} parcelas</div>
                                    <div>Restante: R$ ${formatCurrency(remaining)}</div>
                                </div>
                                <div class="progress mt-1" style="height: 5px;">
                                    <div class="progress-bar" style="width: ${percentage}%; background-color: var(--color-secondary);"></div>
                                </div>
                            </div>
                            <div class="d-flex flex-column ms-2">
                                <button class="btn btn-small btn-custom-success mb-1" onclick="payLoanInstallment(${loan.id})">
                                    Pagar
                                </button>
                                <button class="btn btn-small btn-custom-warning" onclick="showEditLoanModal(${loan.id})">
                                    Editar
                                </button>
                            </div>
                        </div>
                    </div>
                `;
            });
            
            container.innerHTML = html;
        }

        function payLoanInstallment(loanId) {
            const loan = financialData.loans.find(l => l.id === loanId);
            if (loan && loan.paidInstallments < loan.totalInstallments) {
                loan.paidInstallments++;
                saveToFirebase('loans', financialData.loans);
                showToast('Parcela do empréstimo paga!', 'success');
            } else {
                showToast('Todas as parcelas já foram pagas!', 'info');
            }
        }

        function showEditLoanModal(loanId) {
            const loan = financialData.loans.find(l => l.id === loanId);
            if (!loan) return;
            
            const modalBody = `
                <div class="mb-3">
                    <label class="form-label">Nome do Empréstimo:</label>
                    <input type="text" id="editLoanName" class="form-control" value="${loan.name}">
                </div>
                <div class="mb-3">
                    <label class="form-label">Parcelas Pagas:</label>
                    <input type="number" id="editLoanPaid" class="form-control" value="${loan.paidInstallments}">
                </div>
                <div class="mb-3">
                    <label class="form-label">Total de Parcelas:</label>
                    <input type="number" id="editLoanTotal" class="form-control" value="${loan.totalInstallments}">
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancelar</button>
                    <button type="button" class="btn btn-custom-warning" onclick="deleteLoan(${loan.id})">Excluir</button>
                    <button type="button" class="btn btn-custom-primary" onclick="saveLoanEdit(${loan.id})">Salvar</button>
                </div>
            `;
            
            document.getElementById('editLoanModalBody').innerHTML = modalBody;
            new bootstrap.Modal(document.getElementById('editLoanModal')).show();
        }

        function saveLoanEdit(loanId) {
            const loan = financialData.loans.find(l => l.id === loanId);
            if (!loan) return;
            
            loan.name = document.getElementById('editLoanName').value;
            loan.paidInstallments = parseInt(document.getElementById('editLoanPaid').value) || 0;
            loan.totalInstallments = parseInt(document.getElementById('editLoanTotal').value) || 0;
            
            saveToFirebase('loans', financialData.loans);
            bootstrap.Modal.getInstance(document.getElementById('editLoanModal')).hide();
            showToast('Empréstimo atualizado!', 'success');
        }

        function deleteLoan(loanId) {
            if (confirm('Tem certeza que deseja excluir este empréstimo?')) {
                financialData.loans = financialData.loans.filter(l => l.id !== loanId);
                saveToFirebase('loans', financialData.loans);
                bootstrap.Modal.getInstance(document.getElementById('editLoanModal')).hide();
                showToast('Empréstimo excluído!', 'info');
            }
        }

        // Funções para Cartão de Crédito
        function showAddCreditExpenseModal() {
            new bootstrap.Modal(document.getElementById('addCreditExpenseModal')).show();
        }

        function addNewCreditExpense() {
            const name = document.getElementById('creditExpenseName').value || 'Compra';
            const amount = parseFloat(document.getElementById('creditExpenseAmount').value) || 0;
            const date = document.getElementById('creditExpenseDate').value;
            
            if (amount <= 0) {
                showToast('Informe um valor válido!', 'danger');
                return;
            }
            
            const newExpense = {
                id: Date.now(),
                name: name,
                amount: amount,
                date: date,
                type: 'credit'
            };
            
            financialData.creditCard.push(newExpense);
            saveToFirebase('creditCard', financialData.creditCard);
            
            bootstrap.Modal.getInstance(document.getElementById('addCreditExpenseModal')).hide();
            showToast('Despesa no cartão adicionada!', 'success');
        }

        function renderCreditCard() {
            const container = document.getElementById('creditCardContainer');
            const currentMonth = new Date().toISOString().substring(0, 7);
            
            if (!financialData.creditCard || financialData.creditCard.length === 0) {
                container.innerHTML = '<p class="text-muted text-center" style="font-size: 0.9rem;">Nenhuma despesa no cartão</p>';
                document.getElementById('creditCardTotal').textContent = '0,00';
                return;
            }
            
            // Filtrar despesas do mês atual
            const currentMonthExpenses = financialData.creditCard.filter(e => e.date && e.date.substring(0, 7) === currentMonth);
            const total = currentMonthExpenses.reduce((sum, exp) => sum + exp.amount, 0);
            
            document.getElementById('creditCardTotal').textContent = formatCurrency(total);
            
            if (currentMonthExpenses.length === 0) {
                container.innerHTML = '<p class="text-muted text-center" style="font-size: 0.9rem;">Nenhuma despesa este mês</p>';
                return;
            }
            
            let html = '';
            
            currentMonthExpenses.forEach(expense => {
                html += `
                    <div class="expense-item">
                        <div class="d-flex justify-content-between align-items-center">
                            <div>
                                <strong style="font-size: 0.9rem;">${expense.name}</strong>
                                <div style="font-size: 0.8rem; color: #666;">${expense.date}</div>
                            </div>
                            <div>
                                <span style="font-weight: 600; color: var(--color-danger);">R$ ${formatCurrency(expense.amount)}</span>
                                <button class="btn btn-sm btn-link text-danger p-0 ms-2" onclick="deleteCreditExpense(${expense.id})" title="Excluir">
                                    ×
                                </button>
                            </div>
                        </div>
                    </div>
                `;
            });
            
            container.innerHTML = html;
        }

        function deleteCreditExpense(expenseId) {
            financialData.creditCard = financialData.creditCard.filter(e => e.id !== expenseId);
            saveToFirebase('creditCard', financialData.creditCard);
            showToast('Despesa excluída!', 'info');
        }

        // Funções para Despesas Gerais
        function showAddExpenseModal() {
            new bootstrap.Modal(document.getElementById('addExpenseModal')).show();
        }

        function addNewExpense() {
            const name = document.getElementById('expenseName').value || 'Despesa';
            const amount = parseFloat(document.getElementById('expenseAmount').value) || 0;
            const category = document.getElementById('expenseCategory').value;
            const date = document.getElementById('expenseDate').value;
            
            if (amount <= 0) {
                showToast('Informe um valor válido!', 'danger');
                return;
            }
            
            const newExpense = {
                id: Date.now(),
                name: name,
                amount: amount,
                category: category,
                date: date,
                type: 'general'
            };
            
            financialData.generalExpenses.push(newExpense);
            saveToFirebase('generalExpenses', financialData.generalExpenses);
            
            bootstrap.Modal.getInstance(document.getElementById('addExpenseModal')).hide();
            showToast('Despesa adicionada!', 'success');
        }

        function renderGeneralExpenses() {
            const container = document.getElementById('expensesContainer');
            const currentMonth = new Date().toISOString().substring(0, 7);
            
            if (!financialData.generalExpenses || financialData.generalExpenses.length === 0) {
                container.innerHTML = '<p class="text-muted text-center" style="font-size: 0.9rem;">Nenhuma despesa geral</p>';
                document.getElementById('expensesTotal').textContent = '0,00';
                return;
            }
            
            // Filtrar despesas do mês atual
            const currentMonthExpenses = financialData.generalExpenses.filter(e => e.date && e.date.substring(0, 7) === currentMonth);
            const total = currentMonthExpenses.reduce((sum, exp) => sum + exp.amount, 0);
            
            document.getElementById('expensesTotal').textContent = formatCurrency(total);
            
            if (currentMonthExpenses.length === 0) {
                container.innerHTML = '<p class="text-muted text-center" style="font-size: 0.9rem;">Nenhuma despesa este mês</p>';
                return;
            }
            
            let html = '';
            
            currentMonthExpenses.forEach(expense => {
                const categoryNames = {
                    'alimentacao': '🍔 Alimentação',
                    'transporte': '🚗 Transporte',
                    'lazer': '🎮 Lazer',
                    'saude': '🏥 Saúde',
                    'outros': '📦 Outros'
                };
                
                html += `
                    <div class="expense-item">
                        <div class="d-flex justify-content-between align-items-center">
                            <div>
                                <strong style="font-size: 0.9rem;">${expense.name}</strong>
                                <div style="font-size: 0.8rem; color: #666;">
                                    ${categoryNames[expense.category] || 'Outros'} • ${expense.date}
                                </div>
                            </div>
                            <div>
                                <span style="font-weight: 600; color: var(--color-warning);">R$ ${formatCurrency(expense.amount)}</span>
                                <button class="btn btn-sm btn-link text-danger p-0 ms-2" onclick="deleteGeneralExpense(${expense.id})" title="Excluir">
                                    ×
                                </button>
                            </div>
                        </div>
                    </div>
                `;
            });
            
            container.innerHTML = html;
        }

        function deleteGeneralExpense(expenseId) {
            financialData.generalExpenses = financialData.generalExpenses.filter(e => e.id !== expenseId);
            saveToFirebase('generalExpenses', financialData.generalExpenses);
            showToast('Despesa excluída!', 'info');
        }

        // Resumo Financeiro
        function updateResumo() {
            // Apartamento total (financiamento + entrada + despesas)
            const aptFinancing = financialData.apartment.installmentValue;
            const entryFinancing = financialData.entry.installmentValue;
            const aptExpenses = financialData.expenses.condominium + 
                               financialData.expenses.water + 
                               financialData.expenses.energy;
            const aptTotal = aptFinancing + entryFinancing + aptExpenses;
            
            // Carro
            const carTotal = financialData.car.installmentValue;
            
            // Empréstimos
            const loansTotal = (financialData.loans || []).reduce((sum, loan) => {
                return loan.paidInstallments < loan.totalInstallments ? sum + loan.monthlyPayment : sum;
            }, 0);
            
            // Cartão de crédito (mês atual)
            const currentMonth = new Date().toISOString().substring(0, 7);
            const creditCardTotal = (financialData.creditCard || [])
                .filter(e => e.date && e.date.substring(0, 7) === currentMonth)
                .reduce((sum, exp) => sum + exp.amount, 0);
            
            // Despesas gerais (mês atual)
            const expensesTotal = (financialData.generalExpenses || [])
                .filter(e => e.date && e.date.substring(0, 7) === currentMonth)
                .reduce((sum, exp) => sum + exp.amount, 0);
            
            // Total geral
            const totalGeral = aptTotal + carTotal + loansTotal + creditCardTotal + expensesTotal;
            
            // Atualizar interface
            document.getElementById('resumoApartment').textContent = formatCurrency(aptTotal);
            document.getElementById('resumoCar').textContent = formatCurrency(carTotal);
            document.getElementById('resumoLoans').textContent = formatCurrency(loansTotal);
            document.getElementById('resumoCredit').textContent = formatCurrency(creditCardTotal);
            document.getElementById('resumoExpenses').textContent = formatCurrency(expensesTotal);
            document.getElementById('resumoTotal').textContent = formatCurrency(totalGeral);
            
            // Parcelas restantes
            document.getElementById('resumoAptoRestantes').textContent = 
                financialData.apartment.totalInstallments - financialData.apartment.paidInstallments;
            document.getElementById('resumoCarroRestantes').textContent = 
                financialData.car.totalInstallments - financialData.car.paidInstallments;
            
            // Economia (quando concluir parcelas)
            const economia = 0; // Implementar lógica se necessário
            document.getElementById('resumoEconomia').textContent = formatCurrency(economia);
        }

        // Firebase Functions
        function saveToFirebase(path, data) {
            database.ref(path).set(data)
                .then(() => {
                    updateDataStatus('success');
                })
                .catch(error => {
                    console.error('Erro ao salvar no Firebase:', error);
                    updateDataStatus('error');
                    showToast('Erro ao salvar dados!', 'danger');
                });
        }

        function updateAllDisplays() {
            updateApartmentDisplay();
            updateEntryDisplay();
            updateCarDisplay();
            updateExpensesDisplay();
            renderLoans();
            renderCreditCard();
            renderGeneralExpenses();
            updateResumo();
        }

        // Utilitários
        function formatCurrency(value) {
            return value.toFixed(2).replace('.', ',');
        }

        function showToast(message, type) {
            const toast = document.createElement('div');
            toast.className = `alert alert-${type} alert-dismissible fade show`;
            toast.style.cssText = 'animation: slideIn 0.3s ease;';
            toast.innerHTML = `
                ${message}
                <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
            `;
            
            document.getElementById('toastContainer').appendChild(toast);
            
            setTimeout(() => {
                if (toast.parentNode) {
                    toast.remove();
                }
            }, 3000);
        }

        function updateTime() {
            const now = new Date();
            const timeString = now.getHours().toString().padStart(2, '0') + ':' + 
                             now.getMinutes().toString().padStart(2, '0');
            document.getElementById('updateTime').textContent = timeString;
        }

        function updateDataStatus(status) {
            const element = document.getElementById('dataStatus');
            if (status === 'success') {
                element.innerHTML = '🟢 Dados sincronizados';
                element.style.color = 'var(--color-primary)';
            } else {
                element.innerHTML = '🔴 Erro na sincronização';
                element.style.color = 'var(--color-danger)';
            }
        }

        function exportData() {
            const dataStr = JSON.stringify(financialData, null, 2);
            const dataUri = 'data:application/json;charset=utf-8,'+ encodeURIComponent(dataStr);
            const linkElement = document.createElement('a');
            linkElement.setAttribute('href', dataUri);
            linkElement.setAttribute('download', 'controle-financeiro-backup.json');
            linkElement.click();
            showToast('Dados exportados com sucesso!', 'success');
        }

        // Inicializar com dados padrão se Firebase estiver vazio
        function initializeDefaultData() {
            // Esta função pode ser usada para popular dados iniciais
            // Chamar manualmente se necessário
        }
    </script>
</body>
</html>
